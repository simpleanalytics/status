---
title: Status page
---

As a transparent company, we also share our incidents. Please let us know if anything is broken via <a href="mailto:{{ site.email }}">our email</a>. With us you don't see days and days with *"No issues today"*. We just show the all incidents. No ways to trick you, we are not flawless.

> Please contact us if anything is not working correctly via <a href="mailto:{{ site.email }}">email</a> or <a href="https://twitter.com/{{ site.twitter_username }}">twitter</a>

{% for incident in site.incidents | reverse %}
  <h3><a href="{{ incident.url }}">{{ incident.title }}</a></h3>
  <p>
    <span class="label {{ incident.status }}">{{ incident.status }}</span>
    <span class="text-muted">{{ incident.date | date: '%b %d, %Y  %l:%M %P' }} UTC</span>
    {{ incident.excerpt | replace: '<p>','' | replace: '</p>','' }}
    <a href="{{ incident.url }}">Read more</a>.
  </p>
{% endfor %}
