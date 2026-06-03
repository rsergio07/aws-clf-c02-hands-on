# 09 - Service Recognition

## Objective

Develop the ability to quickly identify the correct AWS service based on a business requirement.

Many CLF-C02 questions are service-recognition questions rather than implementation questions.

Estimated time: 15-20 minutes

---

## Storage

### Amazon S3

Use when:

* Storing files
* Backups
* Static websites
* Object storage

Keywords:

```text id="v7m2k5"
Bucket
Object
Durability
Storage
```

---

## Compute

### Amazon EC2

Use when:

* Virtual machines are required
* Full operating system control is needed

Keywords:

```text id="m3r8t1"
Virtual Server
Compute
Instance
AMI
```

---

## Databases

### Amazon RDS

Use when:

* Relational database
* Managed database
* Automated backups

Keywords:

```text id="k8p4v2"
MySQL
PostgreSQL
Multi-AZ
Read Replica
```

---

## Networking

### Amazon VPC

Use when:

* Private network
* Subnets
* Network isolation

Keywords:

```text id="r5n9m7"
VPC
Subnet
Route Table
Internet Gateway
```

---

### Route 53

Use when:

* DNS management
* Domain registration
* Traffic routing

Keywords:

```text id="c1q6t4"
DNS
Domain
Routing
```

---

### CloudFront

Use when:

* Content delivery
* Global caching
* Low latency

Keywords:

```text id="f9m3k8"
CDN
Edge Locations
Caching
```

---

## Security

### IAM

Use when:

* Identity management
* Access control
* Permissions

Keywords:

```text id="d4v8r1"
Users
Groups
Policies
Permissions
```

---

### AWS KMS

Use when:

* Encryption keys
* Cryptographic key management

Keywords:

```text id="h2n5p9"
Encryption
Keys
Data Protection
```

---

### AWS WAF

Use when:

* Protecting web applications
* Filtering HTTP requests

Keywords:

```text id="z8r1m6"
Web Firewall
HTTP Filtering
```

---

### AWS Shield

Use when:

* DDoS protection

Keywords:

```text id="q5k7t3"
DDoS
Network Attacks
```

---

## Monitoring and Governance

### AWS CloudTrail

Use when:

* Auditing API activity
* Investigating user actions

Keywords:

```text id="u4m8n2"
Audit
API Calls
Governance
```

---

### AWS Config

Use when:

* Tracking configuration changes
* Compliance monitoring

Keywords:

```text id="p7r3v5"
Configuration History
Compliance
```

---

### AWS Trusted Advisor

Use when:

* Cost recommendations
* Security recommendations
* Best practices

Keywords:

```text id="y1m6k8"
Recommendations
Optimization
Best Practices
```

---

### AWS Health Dashboard

Use when:

* AWS service disruptions
* Account-specific AWS events

Keywords:

```text id="b3q9t4"
Outages
Service Health
Maintenance
```

---

## Scaling and Availability

### Elastic Load Balancing (ELB)

Use when:

* Distributing traffic
* Improving availability

Keywords:

```text id="g5v2m7"
Load Balancer
Traffic Distribution
```

---

### Auto Scaling

Use when:

* Automatically adjusting capacity

Keywords:

```text id="n8r4p1"
Elasticity
Automatic Scaling
Demand Changes
```

---

## Multi-Account Management

### AWS Organizations

Use when:

* Managing multiple AWS accounts
* Consolidated billing
* Governance

Keywords:

```text id="x4m7k2"
Organizations
Accounts
Governance
```

---

## Compliance

### AWS Artifact

Use when:

* Compliance reports
* Audit documentation

Keywords:

```text id="t9p3v6"
SOC Reports
ISO Reports
Compliance
```

---

## 60-Second Recognition Drill

| Requirement                 | Service             |
| --------------------------- | ------------------- |
| Object Storage              | Amazon S3           |
| Virtual Machine             | Amazon EC2          |
| Managed Relational Database | Amazon RDS          |
| DNS Service                 | Route 53            |
| CDN                         | CloudFront          |
| Identity Management         | IAM                 |
| Encryption Keys             | AWS KMS             |
| DDoS Protection             | AWS Shield          |
| Web Application Firewall    | AWS WAF             |
| API Audit Logs              | AWS CloudTrail      |
| Configuration Tracking      | AWS Config          |
| Cost Recommendations        | AWS Trusted Advisor |
| Account Governance          | AWS Organizations   |
| Load Balancing              | ELB                 |
| Automatic Scaling           | Auto Scaling        |
| Compliance Reports          | AWS Artifact        |

---

## Exam Tip

When answering CLF-C02 questions:

1. Identify the business requirement.
2. Ignore unnecessary technical details.
3. Match the requirement to the AWS service that was specifically designed to solve it.

Many questions can be answered correctly through service recognition alone.

---

## CLF-C02 Concepts Reinforced

* Service Recognition
* Security Services
* Networking Services
* Governance Services
* Monitoring Services
* Global Infrastructure
* Scalability
* High Availability
* Compliance
