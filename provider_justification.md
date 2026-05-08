# Provider Justification – Cloud Platform Selection for a Linux-Based Startup

**Student:** Olamileye Duduyemi
**Date:** May 2026
**Business Context:** Early-Stage Linux Web Startup

---

## Business Scenario

The business context for this justification is an **early-stage technology startup** based in Nigeria, building a Linux-based web application using open-source technologies (e.g., Node.js, PostgreSQL, Nginx). The team has no existing Microsoft licensing and operates on a lean budget with unpredictable early traffic. The startup expects to scale over 12–24 months as the user base grows.

## Recommended Provider: **AWS (with Compute Savings Plans)**

After verifying both providers using their official pricing calculators, the cost comparison reveals that **AWS and Azure are essentially equal at standard pay-as-you-go rates** — AWS at **$53.55/month** and Azure at **$53.25/month** (a difference of only $0.30). Given this near-identical baseline cost, the recommendation is based on additional strategic factors.

**Ecosystem and tooling maturity.** AWS has the broadest global ecosystem for open-source Linux workloads. Services such as AWS CodePipeline, Elastic Beanstalk, and a vast Marketplace of pre-configured Linux AMIs reduce time-to-market for a startup shipping quickly. For a team running Node.js, Python, or similar open-source stacks, AWS's managed service breadth (Lambda, RDS, SQS) provides a natural growth path within a single provider.

**Savings Plans flexibility.** While both providers offer ~36% discounts on 1-year commitments (bringing costs to AWS $41.57 vs Azure $40.91 — again essentially equal), AWS Compute Savings Plans are more flexible. They apply across instance families and regions automatically, whereas Azure Reserved Instances are locked to a specific VM size. For a startup whose workload profile may shift, this flexibility is valuable.

**Multi-zone cost advantage favours Azure.** The one scenario where Azure clearly wins is multi-availability-zone deployments. Azure charges **$0.00** for cross-zone data transfer within the same region, whereas AWS charges **$0.02/GB round-trip**. For a distributed architecture transferring 1 TB/month across zones, this alone saves $20.30/month ($243.60/year) on Azure.

**When Azure Would Win.** For a Microsoft-centric enterprise with existing Windows Server or SQL Server on-premises licences, **Azure Hybrid Benefit** eliminates licensing costs, making Azure the more economical choice. Azure is also the natural fit for teams already using Microsoft 365, Active Directory, or Azure DevOps.

**Conclusion.** Since costs are effectively identical at this scale, the recommendation to use AWS rests on ecosystem breadth and Savings Plan flexibility for a Linux-based startup. However, either provider is a financially sound choice — the decision should ultimately be driven by the team's existing tooling, compliance requirements, and long-term architecture plans.

---

*Word count: approximately 320 words.*
