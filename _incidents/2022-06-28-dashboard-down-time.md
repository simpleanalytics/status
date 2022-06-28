---
title: Dashboard down time
permalink: /incidents/8
date: 2022-06-27 23:32:00 +0000
status: resolved
---

We had an issue with our dashboard script not loading correctly. We check with [Hyperping](https://hyperping.io/), if our site is up and with many other alerts if the data is coming in. The issue here was that the dashboard data did load, but the JavaScript had a load error. Our uptime alerts missed this.

We are also working with Hyperping to set up an alert for the JavaScript loading.

The issue is resolved on <time datetime="{{ '2022-06-28T05:20:00Z' | date_to_xmlschema }}">{{ '2022-06-28T05:20:00Z' | date: "%Y-%m-%d %H:%M:%S" }} UTC</time>. We didn't miss any data, and our APIs, mobile apps, and other systems kept working normally.

We are very sorry for the inconvenience that might have caused.
