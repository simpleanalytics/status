---
title: Degraded performance
permalink: /incidents/11
date: 2024-12-10 23:03:00 +0000
status: resolved
---

We identified that one of our systems caused certain requests to run extremely slowly, resulting in a large number of timeouts. We’ve implemented a hot fix, and since then, 100% of incoming data has been processed and stored successfully.

In total, about 38% of requests failed over a 9.5-hour period due to this performance issue.

We will continue to monitor the system. A few days after the incident, we switched our load balancer from HAProxy to Traefik, which offered better support for our use case.
