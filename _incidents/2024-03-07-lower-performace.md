---
title: Degraded performance
permalink: /incidents/9
date: 2024-03-07 17:50:00 +0000
status: resolved
---

We experienced some disruptions due to an influx of data at an unusually high volume. This occurred because a customer was sending data for numerous users every second. While we do have mechanisms to mitigate traffic from specific domains effectively, we managed to resolve the issue by <time datetime="{{ '2024-03-07T18:56:00Z' | date_to_xmlschema }}">{{ '2024-03-07T18:56:00Z' | date: "%Y-%m-%d %H:%M:%S" }} UTC</time>.

During the hour of service interruption, we were unable to capture 44.3% of the visits. This estimation is derived from our internal benchmarks, which include sending a request to our API every second. We extend our sincerest apologies for any inconvenience this may have caused. To prevent a recurrence, we've enhanced our blocking system to exclude data already present in our queues from being processed.
