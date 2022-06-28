---
title: Status page
---

As a transparent company, we also share our incidents. Please let us know if anything is broken via <a href="mailto:{{ site.email }}">our email</a>. With us you don't see days and days with _"No issues today"_. We just show the all incidents. No ways to trick you, we are not flawless.

> Please contact us if anything is not working correctly via <a href="mailto:{{ site.email }}">email</a> or <a href="https://twitter.com/{{ site.twitter_username }}">twitter</a>

<p>It's currently: <time id="current-time" style="font-feature-settings: 'tnum'; font-variant-numeric: tabular-nums;">loading...</time></p>

{% assign incidents = site.incidents | sort: "date" | reverse %}
{% for incident in incidents %}

  <h3><a href="{{ incident.url }}">{{ incident.title }}</a></h3>
  <p>
    <span class="label {{ incident.status }}">{{ incident.status }}</span>
    <span class="text-muted"><time datetime="{{ incident.date | date_to_xmlschema }}">{{ incident.date | date: "%Y-%m-%d %H:%M:%S" }} UTC</time></span>
    {{ incident.excerpt | replace: '<p>','' | replace: '</p>','' }}
    <a href="{{ incident.url }}">Read more</a>.
  </p>
{% endfor %}
