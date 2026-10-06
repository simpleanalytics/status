---
title: SSL failures for internationalized custom domains
permalink: /incidents/22
date: 2026-09-10
status: resolved
---

From September 10 to October 6, 2026, SSL failures interrupted analytics collection for customers using internationalized custom domains (IDNs), such as domain names containing accented characters. Other custom domains and our default collection endpoints were not affected by this incident.

Our new certificate service compared the Unicode domain names returned by the dashboard with the ASCII (punycode) names used in TLS requests. Although these represent the same domain, the service treated them as different names and rejected valid domains, causing HTTPS connections to fail.

The issue was resolved on October 6 by normalizing both names to the same format before comparison. We're sorry for the disruption and the time it took to identify the issue.
