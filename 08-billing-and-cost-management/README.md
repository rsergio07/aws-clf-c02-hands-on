# 08 - Billing and Cost Management

## Objective

Learn how AWS pricing, billing, budgeting, and cost monitoring work.

By the end of this module, you will be able to:

* Navigate AWS Billing and Cost Management
* Create AWS Budgets
* Use Cost Explorer
* Understand AWS Free Tier
* Recognize common AWS pricing models
* Understand basic support plans

Estimated time: 15-20 minutes

---

## Why This Matters

Cost management is a major topic in the AWS Certified Cloud Practitioner (CLF-C02) exam.

AWS follows a pay-as-you-go model.

Understanding how costs are generated and monitored is essential for both certification and real-world cloud usage.

---

## Key Concepts

### Pay-As-You-Go

With AWS:

```text id="7k2m4q"
Pay only for what you use
```

There are no long-term commitments for most services.

Examples:

* Running EC2 instances
* Storing data in S3
* Running databases in RDS

---

### AWS Free Tier

AWS offers limited free usage for eligible services.

Examples include:

* Amazon EC2
* Amazon S3
* Amazon RDS

Always verify current Free Tier eligibility before creating resources.

---

### AWS Budgets

AWS Budgets allows you to:

* Track spending
* Set cost thresholds
* Receive notifications

Example:

```text id="x8r3n5"
Monthly Budget = $10
```

---

### Cost Explorer

Cost Explorer provides:

* Historical spending
* Forecasting
* Service-level cost breakdowns

Useful for understanding where costs originate.

---

### AWS Support Plans

Common plans:

```text id="q4m7t2"
Basic
Developer
Business
Enterprise On-Ramp
Enterprise
```

For CLF-C02, focus on understanding the purpose of each plan rather than memorizing detailed pricing.

---

## Activity 1 - Explore the Billing Dashboard

Open:

```text id="m5k8v1"
Billing and Cost Management
```

Review:

* Current charges
* Cost summary
* Service breakdown

Expected result:

* Familiarity with billing information

---

## Activity 2 - Create a Budget

Open:

```text id="n2q7f4"
Billing and Cost Management
→ Budgets
```

Create:

```text id="v6r1m9"
Monthly Cost Budget
```

Example:

```text id="c3t8k5"
$10 USD
```

Configure alerts:

```text id="z5m2r8"
80%
100%
```

Expected result:

* Cost monitoring configured

---

## Activity 3 - Explore Cost Explorer

Open:

```text id="p8k4n7"
Cost Explorer
```

Review:

* Service costs
* Time range filters
* Monthly trends

Expected result:

* Understanding of spending visibility

---

## Activity 4 - Review Free Tier Usage

Open:

```text id="f1m6q3"
Billing
→ Free Tier
```

Review:

* Current usage
* Remaining allowance
* Eligible services

Expected result:

* Better understanding of Free Tier limits

---

## Activity 5 - Review AWS Pricing Pages

Explore pricing pages for:

* Amazon EC2
* Amazon S3
* Amazon RDS

Review:

* Pricing units
* Billing dimensions
* Common charges

Expected result:

* Familiarity with AWS pricing models

---

## Activity 6 - Review Support Plans

Open AWS Support documentation.

Compare:

### Basic

Includes:

* Documentation
* AWS Health Dashboard
* Billing support

---

### Developer

Best for:

```text id="g4n8r2"
Development and testing
```

---

### Business

Best for:

```text id="w7m3k1"
Production workloads
```

---

### Enterprise

Best for:

```text id="r2v6q8"
Large organizations
```

Expected result:

* Ability to identify appropriate support plans

---

## Cost Optimization Review

Identify examples of:

* Deleting unused resources
* Using lifecycle policies
* Using managed services
* Monitoring budgets
* Reviewing Cost Explorer

Expected result:

* Awareness of basic AWS cost optimization practices

---

## Common Exam Associations

Understand the relationship between:

| Requirement           | AWS Service         |
| --------------------- | ------------------- |
| Cost tracking         | AWS Budgets         |
| Cost analysis         | Cost Explorer       |
| Usage alerts          | AWS Budgets         |
| Free usage monitoring | Free Tier Dashboard |
| Technical support     | AWS Support Plans   |

---

## Cleanup

No cleanup required.

Keep:

* Budgets
* Billing alerts
* Cost monitoring configurations

These remain useful throughout the rest of the guide.

---

## CLF-C02 Concepts Reinforced

* AWS Pricing
* AWS Free Tier
* AWS Budgets
* Cost Explorer
* Cost Optimization
* AWS Billing
* AWS Support Plans
* Pay-As-You-Go Pricing
* Cloud Financial Management
