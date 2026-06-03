# 06 - Amazon VPC

## Objective

Learn the networking fundamentals of AWS using Amazon Virtual Private Cloud (Amazon VPC).

By the end of this module, you will be able to:

* Understand what a VPC is
* Identify public and private subnets
* Understand route tables
* Understand Internet Gateways
* Recognize how AWS networking components work together

Estimated time: 20-30 minutes

---

## Why VPC Matters

Amazon VPC is the networking foundation for most AWS workloads.

Services such as:

* EC2
* RDS
* Load Balancers
* ECS
* EKS

typically operate inside a VPC.

For CLF-C02, understanding the purpose of each networking component is more important than becoming a networking expert.

---

## Key Concepts

### VPC

A Virtual Private Cloud (VPC) is a logically isolated network within AWS.

Think of it as:

```text id="7p8d3q"
Your private network inside AWS
```

A VPC contains:

* Subnets
* Route tables
* Gateways
* Network resources

---

### Subnet

A subnet is a segment of a VPC.

Common types:

#### Public Subnet

Resources can reach the Internet.

Examples:

```text id="n2q7e1"
Web Servers
Load Balancers
```

---

#### Private Subnet

Resources are not directly accessible from the Internet.

Examples:

```text id="g8r4t6"
Databases
Internal Services
```

---

### Route Table

Determines where network traffic is sent.

Example:

```text id="e3k1v7"
Destination: 0.0.0.0/0
Target: Internet Gateway
```

---

### Internet Gateway

Allows communication between a VPC and the Internet.

Without an Internet Gateway:

```text id="s4v2m8"
No public Internet access
```

---

### Availability Zone

A subnet exists within a specific Availability Zone.

Example:

```text id="j6r9f4"
us-east-1a
us-east-1b
```

Multiple Availability Zones improve resilience.

---

## Activity 1 - Review the Default VPC

Open:

```text id="t7b4d2"
VPC
→ Your VPCs
```

Identify:

* Default VPC
* CIDR block
* Region

Expected result:

* Familiarity with the default network

---

## Activity 2 - Explore Subnets

Open:

```text id="v9m1q6"
VPC
→ Subnets
```

Review:

* Subnet IDs
* Availability Zones
* CIDR blocks

Expected result:

* Understanding of subnet placement

---

## Activity 3 - Review Route Tables

Open:

```text id="p5k8s3"
VPC
→ Route Tables
```

Inspect routes.

Look for:

```text id="r1t6n4"
0.0.0.0/0
```

Expected result:

* Understanding of Internet routing

---

## Activity 4 - Review the Internet Gateway

Open:

```text id="y4f2h8"
VPC
→ Internet Gateways
```

Review:

* Attached VPC
* Gateway configuration

Expected result:

* Understanding how Internet access is enabled

---

## Activity 5 - Review an EC2 Instance Network Configuration

Open:

```text id="d8v3k5"
EC2
→ Instances
→ Networking
```

Review:

* VPC ID
* Subnet ID
* Public IP
* Private IP
* Security Group

Expected result:

* Connect EC2 concepts to VPC concepts

---

## Activity 6 - Create a Custom VPC (Optional)

Create:

```text id="k3n8r7"
CIDR: 10.0.0.0/16
```

Create:

```text id="c5m2p9"
Public Subnet
Private Subnet
```

Expected result:

* Hands-on exposure to VPC creation

---

## Activity 7 - Use AWS CLI

List VPCs:

```bash id="a6w3k1"
aws ec2 describe-vpcs
```

List subnets:

```bash id="q8t4f6"
aws ec2 describe-subnets
```

List route tables:

```bash id="z2m7r5"
aws ec2 describe-route-tables
```

List Internet Gateways:

```bash id="b4x9s8"
aws ec2 describe-internet-gateways
```

Expected result:

* Ability to inspect AWS networking resources programmatically

---

## Console vs CLI

Use the Console when:

* Learning networking concepts
* Visualizing relationships
* Exploring configurations

Use the CLI when:

* Auditing resources
* Automating inventory collection
* Scripting administrative tasks

---

## Cleanup

If a custom VPC was created:

Delete:

* EC2 instances
* Subnets
* Route tables
* Internet Gateway
* VPC

Expected result:

* No unnecessary networking resources remain

---

## CLF-C02 Concepts Reinforced

* Amazon VPC
* Public Subnets
* Private Subnets
* Route Tables
* Internet Gateway
* Availability Zones
* AWS Regions
* Network Isolation
* AWS Global Infrastructure
* AWS CLI
