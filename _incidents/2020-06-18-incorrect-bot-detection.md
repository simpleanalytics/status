---
title: Incorrect bot detection
permalink: /incidents/5
date: 2020-06-18 00:00:00 +0000
status: open
---

On June 18 we updated our public scripts. We did test with a few customers if the same amount of visits ended up in our database. This was the case. What we didn't know was that we classified them as robots. We still store these visits as we want to show our customer how many visits come for robots for a better comparison with other analytics tools.

In your dashboard we don't show these visits yet, we need to migrate them so they will become visible to you. We do this when our public script is updated and the cache is expired for most browsers. When this is done we will set the status of this incident to resolved and remove the tooltip from the charts.
