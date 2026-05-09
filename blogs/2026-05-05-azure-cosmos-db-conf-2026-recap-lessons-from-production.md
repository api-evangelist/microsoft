---
title: "Azure Cosmos DB Conf 2026 Recap: Lessons from Production"
url: "https://devblogs.microsoft.com/blog/azure-cosmos-db-conf-2026-recap-lessons-from-production"
date: "2026-05-05"
author: "Mark Brown"
feed_url: "https://devblogs.microsoft.com/feed/"
---
A team was running at 100% RU utilization. Throttles were compounding into retries. P99 latency was degrading. The assumption was obvious: provision more throughput. They didn’t. Instead, they found a single logical partition absorbing more than 80% of traffic. After fixing the data model—without scaling the database—RU utilization dropped to 20–35%, throttling vanished, and latency normalized. That was the real-world case study Anurag Dutt shared in his Azure Cosmos DB Conf 2026 session, From Rising RU Costs to Stable Performance. One automated integration account was generating most writes.
