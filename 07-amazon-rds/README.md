# 07 - Amazon RDS

## Objective

Learn the fundamentals of Amazon Relational Database Service (Amazon RDS), AWS's managed relational database service.

By the end of this module, you will be able to:

* Understand managed databases
* Launch an RDS instance
* Identify supported database engines
* Understand backups and Multi-AZ deployments
* Recognize common RDS use cases

Estimated time: 20-30 minutes

---

## Why RDS Matters

Amazon RDS allows organizations to run relational databases without managing the underlying infrastructure.

AWS handles:

* Provisioning
* Patching
* Backups
* Monitoring
* High Availability options

For CLF-C02, understanding the value of managed services is more important than database administration.

---

## Key Concepts

### Managed Database

With Amazon RDS:

AWS manages:

* Operating systems
* Hardware
* Database patching
* Automated backups

You manage:

* Database configuration
* Users
* Data

---

### Supported Database Engines

Common engines include:

```text id="t4q9n8"
MySQL
PostgreSQL
MariaDB
Oracle
Microsoft SQL Server
```

Expected exam focus:

* Recognize supported engines
* Understand managed database benefits

---

### Automated Backups

RDS can automatically create backups.

Benefits:

* Point-in-time recovery
* Disaster recovery
* Operational resilience

---

### Multi-AZ Deployment

Creates a standby database in another Availability Zone.

Benefits:

* High availability
* Improved resiliency
* Automatic failover

---

### Read Replicas

Used primarily for:

```text id="y8k2r4"
Read scaling
```

Common exam distinction:

```text id="e5m7v3"
Multi-AZ = Availability
Read Replica = Performance
```

---

## Activity 1 - Explore Amazon RDS

Open:

```text id="w7n4q5"
RDS
→ Databases
```

Review:

* Existing databases
* Database engines
* Status information

Expected result:

* Familiarity with the RDS console

---

## Activity 2 - Create a Database

Create:

```text id="x3m8k1"
MySQL
```

Choose:

```text id="v2r6n7"
Free Tier template
```

Review:

* Engine version
* Storage
* Instance class

Expected result:

* One RDS database instance

---

## Activity 3 - Review Configuration

Review:

* Endpoint
* Availability Zone
* Storage allocation
* Backup settings

Expected result:

* Familiarity with RDS properties

---

## Activity 4 - Review Backup Configuration

Inspect:

```text id="f8q3t6"
Automated Backups
```

Review:

* Retention period
* Recovery options

Expected result:

* Understanding of backup capabilities

---

## Activity 5 - Review High Availability Options

During creation or modification, review:

```text id="r6m9p4"
Multi-AZ Deployment
```

Understand:

* Purpose
* Cost implications
* Availability benefits

Expected result:

* Ability to differentiate HA concepts

---

## Activity 6 - Review Read Replicas

Explore:

```text id="p4v8n2"
Create Read Replica
```

Review:

* Use case
* Performance benefits

Expected result:

* Understanding of read scaling concepts

---

## Activity 7 - Use AWS CLI

List database instances:

```bash id="m9r5q7"
aws rds describe-db-instances
```

List database engines:

```bash id="c2k8t1"
aws rds describe-db-engine-versions
```

Review available engines:

```bash id="b7v3n4"
aws rds describe-orderable-db-instance-options
```

Expected result:

* Ability to inspect RDS resources using AWS CLI

---

## Managed Service Comparison

Understand the difference:

### Amazon EC2

You manage:

* Operating system
* Patching
* Database software
* Backups

---

### Amazon RDS

AWS manages:

* Infrastructure
* Patching
* Backups
* Maintenance

You manage:

* Database configuration
* Users
* Data

Expected result:

* Understanding managed service responsibility boundaries

---

## Cleanup

Delete:

* Test database instances
* Snapshots if not needed

Verify:

```text id="n5w2m8"
Database removed successfully
```

Expected result:

* No unnecessary RDS costs

---

## CLF-C02 Concepts Reinforced

* Managed Services
* Amazon RDS
* Relational Databases
* Automated Backups
* Multi-AZ Deployments
* Read Replicas
* High Availability
* Shared Responsibility Model
* AWS CLI
