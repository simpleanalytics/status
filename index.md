---
title: Status page
---


As a transparent company, we also share our incidents. Please let us know if anything is broken via <a href="mailto:{{ site.email }}">our email</a>. With us you don't see days and days without issues. We just show the most incidents. No ways to trick you, we are not flawless.

{% for incident in site.incidents %}
  <h3><a href="{{ incident.url }}">{{ incident.title }}</a></h3>
  <p>
    <span class="label {{ incident.status }}">{{ incident.status }}</span>
    <span class="text-muted">{{ incident.date | date: '%b %d, %Y  %l:%M %P' }} UTC</span>
    {{ incident.excerpt | replace: '<p>','' | replace: '</p>','' }}
    <a href="{{ incident.url }}">Read more</a>.
  </p>
{% endfor %}
