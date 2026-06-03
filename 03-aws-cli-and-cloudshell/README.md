# 03 - AWS CLI and CloudShell

## Objective

Learn how to interact with AWS using command-line tools instead of relying exclusively on the AWS Management Console.

By the end of this module, you will be able to:

* Configure the AWS CLI
* Verify AWS authentication
* Execute basic AWS commands
* Navigate AWS CloudShell
* Understand when to use the Console, CLI, or CloudShell

Estimated time: 15-20 minutes

---

## Why This Matters

Every action performed in the AWS Console ultimately results in an API call.

The AWS CLI provides direct access to those APIs from a terminal.

Understanding the AWS CLI helps reinforce how AWS services work and introduces skills commonly used in cloud, DevOps, and SRE roles.

---

## Key Concepts

### AWS Console

Best for:

* Learning new services
* Visual exploration
* Resource management
* Occasional administrative tasks

---

### AWS CLI

Best for:

* Automation
* Scripting
* Repetitive tasks
* Bulk operations

---

### AWS CloudShell

Best for:

* Browser-based administration
* Quick testing
* Temporary environments
* AWS access without local setup

CloudShell includes:

* AWS CLI
* Python
* Git
* Common Linux utilities

---

## Activity 1 - Verify AWS CLI Installation

Run:

```bash
aws --version
```

Expected result:

```text
aws-cli/2.x.x
```

---

## Activity 2 - Review AWS CLI Configuration

Run:

```bash
aws configure list
```

Review:

* Access key
* Region
* Output format

Expected result:

* CLI configuration is visible

---

## Activity 3 - Verify Identity

Run:

```bash
aws sts get-caller-identity
```

Expected result:

```json
{
  "UserId": "...",
  "Account": "...",
  "Arn": "..."
}
```

Observe:

* AWS Account ID
* IAM User ARN

---

## Activity 4 - Explore AWS Regions

Run:

```bash
aws ec2 describe-regions
```

Observe:

* Region names
* Geographic distribution
* AWS global infrastructure

Expected result:

* Better understanding of AWS Regions

---

## Activity 5 - Explore IAM Resources

List users:

```bash
aws iam list-users
```

List groups:

```bash
aws iam list-groups
```

Expected result:

* Visibility into IAM resources

---

## Activity 6 - Open AWS CloudShell

From the AWS Console:

```text
CloudShell
```

Launch a CloudShell session.

Run:

```bash
aws sts get-caller-identity
```

Compare the experience between:

* Local AWS CLI
* AWS CloudShell

Expected result:

* Understand the purpose of CloudShell

---

## Activity 7 - Explore S3

Run:

```bash
aws s3 ls
```

Expected result:

* Existing buckets displayed
* Empty result if no buckets exist

This command will be used extensively in the next module.

---

## Common Commands

Current identity:

```bash
aws sts get-caller-identity
```

Current configuration:

```bash
aws configure list
```

List regions:

```bash
aws ec2 describe-regions
```

List IAM users:

```bash
aws iam list-users
```

List IAM groups:

```bash
aws iam list-groups
```

List S3 buckets:

```bash
aws s3 ls
```

---

## Cleanup

No cleanup required.

This module does not create billable resources.

---

## CLF-C02 Concepts Reinforced

* AWS CLI
* AWS APIs
* Programmatic Access
* IAM Authentication
* IAM Authorization
* AWS Regions
* CloudShell
* AWS Global Infrastructure
