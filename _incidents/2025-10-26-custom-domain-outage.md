---
title: Custom domain data ingestion incident
permalink: /incidents/16
date: 2025-10-26 00:00:00 +0000
status: resolved
---

Summary  
We saw intermittent data ingestion for websites sending via a custom domain. A DDoS protection trigger at our hosting platform, Leaseweb, rate limited part of this traffic. The issue is now resolved.

Impact  
- Only customers using a custom collection domain were affected.  
- Ingestion was limited for a total of 54 minutes, some data still arrived during this window.  
- Customers using our default endpoints were not affected.

Root cause  
A DDoS protection rule at Leaseweb incorrectly throttled custom domain traffic.

Resolution  
We worked with Leaseweb to remove the limiting condition, traffic is normal again.

Next steps  
We will move custom domain traffic away from Leaseweb’s DDoS protection, and add safeguards to prevent a repeat.
