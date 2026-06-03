# 05 - Amazon EC2

## Objective

Learn the fundamentals of Amazon Elastic Compute Cloud (Amazon EC2), AWS's primary compute service.

By the end of this module, you will be able to:

* Launch an EC2 instance
* Understand instance types
* Configure security groups
* Connect to an instance
* Stop and terminate instances
* Understand common EC2 pricing concepts

Estimated time: 30-45 minutes

---

## Why EC2 Matters

Amazon EC2 provides virtual servers in the cloud.

Many AWS workloads run on EC2.

Common use cases include:

* Web servers
* Application servers
* Development environments
* Legacy applications
* Self-managed databases

For CLF-C02, EC2 is one of the most frequently referenced services.

---

## Key Concepts

### Instance

An EC2 instance is a virtual machine running in AWS.

Examples:

```text id="d4v2s7"
Web Server
Application Server
Linux Development Host
```

---

### Instance Type

Defines:

* CPU
* Memory
* Network performance

Examples:

```text id="6x6a7y"
t2.micro
t3.micro
t4g.micro
```

For practice, use Free Tier eligible options when available.

---

### AMI

Amazon Machine Image.

Defines the operating system and initial configuration.

Examples:

```text id="m3c8o4"
Amazon Linux
Ubuntu
Windows Server
```

---

### Security Group

Acts as a virtual firewall.

Controls:

* Inbound traffic
* Outbound traffic

Example:

```text id="j7x9e5"
Allow SSH (22)
Allow HTTP (80)
```

---

### Key Pair

Used for secure instance access.

Required for:

* SSH access to Linux instances

Always store private keys securely.

---

## Activity 1 - Launch an EC2 Instance

Open:

```text id="n9q4x2"
EC2
→ Launch Instance
```

Configuration:

```text id="q4t1c6"
Amazon Linux
t2.micro or t3.micro
Default VPC
```

Expected result:

* One running EC2 instance

---

## Activity 2 - Review Instance Details

Review:

* Instance ID
* Public IP
* Private IP
* Availability Zone
* Instance type

Expected result:

* Familiarity with EC2 properties

---

## Activity 3 - Review Security Groups

Open:

```text id="z2s5g7"
Instance
→ Security
→ Security Group
```

Review:

* Inbound rules
* Outbound rules

Expected result:

* Understanding of basic network controls

---

## Activity 4 - Connect to the Instance

Use:

```text id="t8w4b9"
EC2 Instance Connect
```

or

```text id="e7r1h3"
SSH
```

Run:

```bash id="g6k3r8"
hostname
```

Run:

```bash id="s5m8q2"
uname -a
```

Expected result:

* Successful connection

---

## Activity 5 - Stop and Start the Instance

Perform:

```text id="w4b7x1"
Stop Instance
Start Instance
```

Observe:

* State transitions
* Public IP changes (if applicable)

Expected result:

* Familiarity with EC2 lifecycle states

---

## Activity 6 - Explore Instance Pricing

Review:

```text id="p3k9d4"
On-Demand
Reserved Instances
Savings Plans
Spot Instances
```

Understand common use cases for each.

Expected result:

* Better understanding of AWS pricing models

---

## Activity 7 - Use AWS CLI

List instances:

```bash id="x1m7s5"
aws ec2 describe-instances
```

List instance status:

```bash id="r6v2j8"
aws ec2 describe-instance-status
```

Start an instance:

```bash id="h5p8q4"
aws ec2 start-instances --instance-ids INSTANCE_ID
```

Stop an instance:

```bash id="b4d6k7"
aws ec2 stop-instances --instance-ids INSTANCE_ID
```

Expected result:

* Basic EC2 management using AWS CLI

---

## Console vs CLI

Use the Console when:

* Learning EC2
* Reviewing configuration
* Launching new instances

Use the CLI when:

* Automating administration
* Managing multiple instances
* Creating repeatable workflows

---

## Cleanup

Terminate the test instance.

Verify:

```text id="f8t2m5"
Instance State = Terminated
```

Remove:

* Unused security groups
* Unused key pairs

Expected result:

* No unnecessary EC2 resources remain

---

## CLF-C02 Concepts Reinforced

* Compute
* Virtual Machines
* EC2 Instances
* AMIs
* Security Groups
* Key Pairs
* Availability Zones
* On-Demand Pricing
* Spot Instances
* Savings Plans
* AWS CLI
