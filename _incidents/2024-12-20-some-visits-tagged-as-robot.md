---
title: Some visits tagged as robot
permalink: /incidents/12
date: 2024-12-19 13:00:00 +0000
status: resolved
---

We’ve identified that our advanced robot blocking feature is tagging too many visits as robot. We’re currently fixing this issue. No data is lost and it will appear in your dashboard a bit later. Only some users are affected. To verify if your data is coming in (including robots), please export the data with robot information included.

Update: We’ve fixed the issue. All incorrectly tagged robot data has been reclassified as non-robot. The root cause was our new load balancer, which failed to forward IP headers correctly to our queue application. This only affected customers using the advanced robot blocking feature. Incoming traffic is now processed correctly, and historical data is also fixed. The advanced robot blocking feature will be fully functional after the weekend. We’re holding off on any new updates for now.
