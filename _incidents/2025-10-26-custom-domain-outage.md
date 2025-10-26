---
title: Custom domain data ingestion incident
permalink: /incidents/16
date: 2025-10-26 00:00:00 +0000
status: identified
---

We are seeing intermittent data ingestion for websites that send data via a custom domain.  
A DDoS protection trigger at our hosting platform, Leaseweb, is rate limiting part of this traffic.

Impact
- Only customers using a custom collection domain are affected.  
- Some data from custom domains is still coming in, but ingestion is degraded.  
- Customers using our default endpoints are not affected.

Current status
We have identified the Leaseweb DDoS trigger and are in contact with their team to restore full throughput. We will update this page as we make progress.

Next steps
We are tuning our network rules with Leaseweb and adding safeguards to prevent a repeat.
