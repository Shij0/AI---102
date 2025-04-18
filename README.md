# AI---102

You have an Azure Cognitive Search service.
During the past 12 months, query volume steadily increased.
You discover that some search query requests to the Cognitive Search service are being throttled.
You need to reduce the likelihood that search query requests are throttled.
Solution: You migrate to a Cognitive Search service that uses a higher tier.
Does this meet the goal?

A. Yes
B. No

Answer:

**A. Yes**

**Explanation:**

Migrating to a higher tier for your Azure Cognitive Search service (now **Azure AI Search**) **does meet the goal** of reducing the likelihood of search query requests being throttled due to increased query volume.

Here's why:

* **Throttling:** Throttling in Azure AI Search occurs when the service exceeds its capacity to handle incoming query requests. This capacity is determined by the service's pricing tier and the number of replicas and partitions.
* **Higher Tiers:** Higher pricing tiers in Azure AI Search offer increased limits on queries per second (QPS) and typically provide access to more replicas and partitions (which further increase QPS handling capacity and throughput).

By migrating to a tier with a higher inherent QPS limit and the ability to scale out with more replicas, your search service will be able to handle a significantly larger volume of search query requests before reaching its capacity and triggering throttling. This directly addresses the problem of throttling caused by increased query volume.


Question #: 22
Topic #: 1

You have an Azure Cognitive Search service.
During the past 12 months, query volume steadily increased.
You discover that some search query requests to the Cognitive Search service are being throttled.
You need to reduce the likelihood that search query requests are throttled.
Solution: You migrate to a Cognitive Search service that uses a higher tier.
Does this meet the goal?

A. Yes
B. No

**A. Yes**

**Explanation:**

Migrating to a higher tier for your Azure Cognitive Search service (now **Azure AI Search**) **does meet the goal** of reducing the likelihood of search query requests being throttled due to increased query volume.

Here's why:

* **Increased Capacity Limits:** Each tier in Azure AI Search has different resource allocations and limits on factors like queries per second (QPS), storage, and the maximum number of replicas and partitions you can configure. Higher tiers provide significantly higher base QPS limits and allow you to scale out to a greater extent by adding more replicas.
* **Throttling Mechanism:** Throttling occurs when your search service is unable to handle the incoming query load with its current configuration (tier, replicas, and partitions).
* **Reducing Likelihood:** By moving to a higher tier, you are increasing the overall processing capacity available to your search service. This means the service can handle a larger volume of concurrent queries before hitting its limits and starting to throttle requests. While adding replicas is the primary way to scale *query throughput* within a tier, migrating to a higher tier is often a necessary step to *enable* adding enough replicas to handle significantly increased volume, and it also provides a higher baseline capacity.

Therefore, by increasing the service's fundamental capacity and potential for scaling, migrating to a higher tier directly contributes to reducing the probability that incoming search query requests will be throttled when the query volume increases.


