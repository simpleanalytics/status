---
title: Dashboard down time
permalink: /incidents/8
date: 2022-06-27 23:32:00 +0000
status: resolved
---

We had an issue with our dashboard script not loading correctly. We do check with [hyperping.io](https://hyperping.io/), if our site is up and with many other alerts if the data is coming in. The issue here was that the dashboard data did load, but the JavaScript had a load error. This wasn't catched by our uptime alerts.

We are working with Hyperping to setup an alert for the JavaScript loading as well.

The issue is resolved at 2022-06-28 05:20:00 UTC. We didn't miss any data, our APIs, mobile apps, and other systems kept working normally.

We are very sorry for the inconvenience that might have caused.
