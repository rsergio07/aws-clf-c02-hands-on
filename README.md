# AWS Cloud Practitioner Practical Guide

A practical, hands-on guide for learning AWS while preparing for the AWS Certified Cloud Practitioner (CLF-C02) certification.

This repository focuses on real AWS usage rather than theory. The goal is to reinforce core cloud concepts by creating, managing, and cleaning up AWS resources using the AWS Management Console, AWS CLI, and basic Infrastructure as Code.

## Objectives

* Build practical familiarity with core AWS services.
* Reinforce CLF-C02 concepts through repetition and experimentation.
* Develop confidence navigating the AWS Console and AWS CLI.
* Understand AWS security, pricing, and operational fundamentals.
* Create a reusable personal reference for future AWS certifications.

## Target Certification

* AWS Certified Cloud Practitioner (CLF-C02)

## Learning Approach

Each section focuses on a specific AWS service or domain and includes:

* Service overview
* Key CLF-C02 concepts
* Hands-on activities
* AWS CLI examples
* Cleanup procedures
* Cost awareness notes
* Personal observations and lessons learned

## Repository Structure

```text
.
├── README.md
├── iam/
├── cli/
├── s3/
├── ec2/
├── vpc/
├── rds/
├── billing/
└── notes/
```

## Covered Topics

### Security and Identity

* AWS Account
* IAM Users
* IAM Groups
* IAM Policies
* MFA
* Least Privilege

### Cloud Operations

* AWS CLI
* AWS CloudShell
* Regions and Availability Zones

### Storage

* Amazon S3
* Storage Classes
* Versioning
* Lifecycle Policies

### Compute

* Amazon EC2
* Security Groups
* Key Pairs

### Networking

* Amazon VPC
* Subnets
* Route Tables
* Internet Gateway

### Databases

* Amazon RDS
* Managed Database Concepts

### Billing and Cost Management

* AWS Budgets
* Cost Explorer
* Free Tier Monitoring

## Cost and Safety Principles

* Always use Free Tier eligible resources when possible.
* Review estimated costs before creating resources.
* Delete resources immediately after completing exercises.
* Configure AWS Budgets and billing alerts before starting labs.
* Never perform daily activities using the root account.

## Disclaimer

This repository is intended for educational purposes and personal skill development. AWS services and pricing change over time; always verify current documentation and pricing before creating resources.
