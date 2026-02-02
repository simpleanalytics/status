---
title: Deploying new dashboard version with minor regressions
permalink: /incidents/19
date: 2026-02-02 13:13:18 +0000
status: resolved
---

We deployed a new version of the dashboard. The following regressions occurred and have been fixed:

- Failed to login when legacy API token was set.
- Export failed for CSV.
- Allow token to be optional for public dashboard live visitors: without login, live pageviews of published dashboards were not visible.
- No proper error when user id was missing prefix in API auth.

Update 14:14 UTC: All regressions have been fixed.
