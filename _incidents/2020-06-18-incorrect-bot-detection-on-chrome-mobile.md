---
title: Incorrect bot detection on Chrome mobile
permalink: /incidents/5
date: 2020-06-18 00:00:00 +0000
status: resolved
---

On June 18 we updated our public scripts. We did test with a few customers if the same amount of visits ended up in our database. This was the case. What we didn't know was that we classified them as robots. We still store these visits as we want to show our customer how many visits came for robots for a better comparison with other analytics tools. It only effects visits from Chrome browsers on mobile. This includes Chrome for Android, Samsung Internet, UC Browser for Android, Microsoft Edge Mobile, and Opera Mobile. **Your visits are not lost**, they just don't show up in the dashboard just yet.

In your dashboard we don't show these visits yet, we need to migrate them so they will become visible to you. We do this after our public script is updated and the cache is expired for most browsers. When this is done we will set the status of this incident to resolved and remove the tooltip from the charts.

For the days between June 18 and now you will see less visits from mobile browsers. This will be corrected in a few days.

Resolved on July 23 to make sure all missed visits are included. For most customers there is almost no difference visible. All data is now correct.
