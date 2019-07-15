---
title: Network outage in data center
permalink: /incidents/1
date: 2019-07-11 18:10:00 +0000
status: resolved
---

As a transparent company, we also share our issues. On July 11th at 6:10 PM UTC we had a network outage in our data center in Iceland. We noticed this promptly with our monitoring systems and quick help from [Daniel](https://twitter.com/DanielLockyer) (our server hero). After 46 minutes our servers were reachable again and the outage was over.

Today we worked hard on getting the data more accurate by using the average of the hour before and after the incident. We used that average to replace the data of the 46 minutes where we were unreachable. The calculation we used for the outage period is: `( ( VISITS 4 to 5PM + VISITS 6 to 7PM ) / 2 )`. This means that we only corrected the visits and no other data.

We do have backup systems in place in case our main server does not function properly, but we didn’t have solutions for a total network outage. We are looking into solutions on how to prevent this from happening ever again. We welcome any feedback on how to prevent this in the  future.

We will spend the next few hours to implement an annotation in our graph to show where exactly the data is a bit off. These annotations will also be used in the future to explain  spikes if we can relate them to specific referrals.

But we also have positive news to share. To name a few:
- This week we reached [$20,000 ARR](https://simpleanalytics.com/open?ref={{ site.hostname }})
- We are also working hard on events which we expect to have live in 4 weeks<br>
  If you want to have early access, [send us a message](https://simpleanalytics.com/contact?ref={{ site.hostname }}).
- We added [a simple Stats API](https://docs.simpleanalytics.com/api?ref={{ site.hostname }}#stats-api) to retrieve your websites data
- We created [docs for you](https://docs.simpleanalytics.com/?ref={{ site.hostname }}) where you can see all our features and how to use them
- We have a [public roadmap](https://simpleanalytics.com/roadmap?ref={{ site.hostname }}) (for a few months now)
- We have the [simpleanalytics.com](https://simpleanalytics.com?ref={{ site.hostname }}) domain!

Anyhow, we keep on working hard on being the best privacy friendly analytics tool out there. Sorry again and thank you for your support which keeps us motivated to  work on something as cool as Simple Analytics.
