# AWS CLI

## Purpose

The AWS Command Line Interface (AWS CLI) provides a unified tool to manage AWS services directly from the terminal.

Learning the AWS CLI helps reinforce AWS concepts, improves productivity, and builds skills that are commonly used in cloud engineering, DevOps, SRE, and automation roles.

## CLF-C02 Concepts Covered

* AWS CLI
* Programmatic Access
* AWS API Interactions
* Regions
* Credentials
* IAM Permissions
* Authentication and Authorization

## Installation

Verify AWS CLI installation:

```bash
aws --version
```

Expected output:

```text
aws-cli/2.x.x
```

## Configure AWS CLI

Configure credentials:

```bash
aws configure
```

Example:

```text
AWS Access Key ID: ****************
AWS Secret Access Key: ****************
Default region name: us-east-1
Default output format: json
```

Verify configuration:

```bash
aws configure list
```

## Hands-On Activities

### Activity 1 – Verify Identity

Display the currently authenticated user:

```bash
aws sts get-caller-identity
```

Expected result:

* AWS Account ID
* User ARN
* User ID

### Activity 2 – List Available Regions

```bash
aws ec2 describe-regions
```

Observe:

* Region names
* Geographic distribution
* AWS global infrastructure

### Activity 3 – Explore S3

List buckets:

```bash
aws s3 ls
```

Expected result:

* Existing buckets or empty output

### Activity 4 – Explore IAM

List IAM users:

```bash
aws iam list-users
```

Observe:

* IAM usernames
* Creation dates
* Account structure

### Activity 5 – Use CloudShell

Open AWS CloudShell from the AWS Console.

Compare:

* Local terminal
* AWS CloudShell

Identify advantages of each environment.

## When To Use Each Tool

### AWS Console

Use when:

* Learning a service
* Visual exploration
* Reviewing resources
* Performing occasional tasks

### AWS CLI

Use when:

* Automation is needed
* Repeating tasks
* Scripting
* Bulk operations

### AWS CloudShell

Use when:

* Working from a browser
* No local tooling is available
* Quick AWS administration is required

## Common Commands

Current identity:

```bash
aws sts get-caller-identity
```

Current configuration:

```bash
aws configure list
```

List S3 buckets:

```bash
aws s3 ls
```

List IAM users:

```bash
aws iam list-users
```

List regions:

```bash
aws ec2 describe-regions
```

## Cleanup

No cleanup required.

The AWS CLI itself does not create billable resources.

## Key Takeaways

* The AWS CLI communicates directly with AWS APIs.
* IAM permissions determine what commands can be executed.
* AWS CLI is a foundational skill for cloud practitioners.
* CloudShell provides AWS CLI access without local installation.
* Most AWS operations can be performed through either the Console or CLI.
