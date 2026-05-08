# AWS vs Azure Cost Comparison – Repository Overview

**Student:** Olamileye Duduyemi
**Date:** May 2026
**Assignment:** Cloud Economics & Pricing – AWS vs Azure

---

## Repository Contents

| File | Description |
|---|---|
| `cost_comparison_report.md` | Full cost breakdown: compute, storage, egress, networking, discounts, and optimization strategies |
| `provider_justification.md` | ~320-word business context justification for provider selection |
| `README.md` | This file |
| `screenshots/` | Calculator screenshots verifying resource configurations |

---

## Application Specs Used

| Spec | Value |
|---|---|
| Compute | 2 vCPU, 4 GB RAM (Linux) |
| Storage | 128 GB SSD |
| Monthly Egress | 100 GB outbound |
| Region (AWS) | EU-West-1 (Ireland) |
| Region (Azure) | UK South (London) |

---

## Key Findings

| Scenario | AWS | Azure | Cheaper |
|---|---|---|---|
| On-Demand / PAYG | $53.55/mo ✅ | $53.25/mo ✅ | **Essentially equal** (-$0.30) |
| 1-Year Committed | $41.57/mo | $40.91/mo | **Azure** by $0.66 |
| Multi-AZ (+1 TB cross-zone) | $73.55/mo | $53.25/mo | **Azure** by $20.30 |

## Pricing Calculator Links

- 🔗 **AWS Pricing Calculator:** [calculator.aws](https://calculator.aws/)
  - Region: EU (Ireland) | Instance: t3.medium | OS: Linux | EBS: gp3 128 GB
- 🔗 **Azure Pricing Calculator:** [azure.microsoft.com/pricing/calculator](https://azure.microsoft.com/en-gb/pricing/calculator/)
  - Region: UK South | VM: A1 Basic | OS: Linux (Ubuntu) | 730 hours | $34.29/month

## Screenshots

| Screenshot | What It Shows |
|---|---|
| `screenshots/01_aws_calculator.png` | AWS Pricing Calculator configured with t3.medium + EBS gp3 + data transfer |
| `screenshots/02_azure_calculator.png` | Azure Pricing Calculator configured with A1 Basic (1 Core, 1.75 GB RAM), Linux, UK South, 730 hours — $34.29/month |
