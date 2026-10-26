---
title: Server maintenance for security updates
permalink: /incidents/23
date: 2026-10-26 16:00:00 +0000
status: open
---

Between 16:00 and 17:00 UTC today, we're applying security updates to our servers. Some services may be briefly unavailable while they restart. We expect less than 5 minutes of downtime in total.

We'll update this post when the maintenance is done.

**Update 20:50 UTC:** The maintenance took longer than planned. We restarted all our servers and upgraded the software running on them, in response to the [recently disclosed compromise of several eMudhra intermediate certificate authorities](https://emudhra.we-have-a-problem.com/). Our servers no longer trust certificates issued by them. We have no indication that the compromise was used against us.

What you may have noticed (times in UTC):

- **15:45–15:52:** Custom domains returned SSL errors, so visits to websites that load our script through a custom domain were not collected during these minutes.
- **Around 16:10:** Services that run on a single server, such as the live visitor counter, were unavailable for about a minute while that server restarted.
- **From 18:40:** Our database cluster was degraded while it rebalanced after the restarts. During that time, statistics could load slowly or be incomplete, and new data was processed with a delay. The cluster is healthy again.

The cookie scanner is still unavailable. We're working on it and will mark this incident resolved once it's back.
