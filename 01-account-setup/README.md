# 01 - Account Setup

## Objective

Prepare a new AWS account for hands-on practice while minimizing the risk of unexpected charges.

By the end of this module, you will have:

* An AWS account
* Multi-Factor Authentication (MFA) enabled
* Billing alerts configured
* A dedicated IAM administrator user
* AWS CLI installed and ready for use

Estimated time: 15-20 minutes

---

## Prerequisites

Before starting:

* A valid email address
* A phone number
* A credit/debit card
* A computer running macOS, Windows, or Linux

---

## Step 1 - Create an AWS Account

1. Navigate to https://aws.amazon.com/
2. Select **Create an AWS Account**
3. Complete the registration process
4. Choose the **Basic Support Plan**
5. Sign in to the AWS Management Console

Expected result:

* Access to the AWS Console
* Access to the Billing Dashboard

---

## Step 2 - Enable MFA for the Root User

1. Open the AWS Console
2. Select your account name
3. Navigate to **Security Credentials**
4. Locate **Multi-Factor Authentication (MFA)**
5. Configure an authenticator application

Recommended applications:

* Google Authenticator
* Microsoft Authenticator
* Authy

Expected result:

* Root account protected with MFA

---

## Step 3 - Create an IAM Administrator User

Do not use the root account for daily activities.

1. Open IAM
2. Create a new user
3. Enable AWS Management Console access
4. Assign the user to a group with:

```text
AdministratorAccess
```

Expected result:

* Dedicated administrative user
* Ability to sign in without using the root account

---

## Step 4 - Create a Billing Budget

Open:

```text
Billing and Cost Management
```

Create:

```text
Monthly Budget: $10 USD
```

Configure:

```text
80% alert
100% alert
```

Expected result:

* Email notifications when spending reaches configured thresholds

---

## Step 5 - Install AWS CLI

Verify installation:

```bash
aws --version
```

If AWS CLI is not installed, follow the official AWS documentation.

Expected result:

```text
aws-cli/2.x.x
```

---

## Step 6 - Configure AWS CLI

Create an access key for the IAM administrator user.

Configure locally:

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

Verify:

```bash
aws sts get-caller-identity
```

Expected result:

* AWS Account ID
* IAM User ARN

---

## Validation Checklist

Before continuing, confirm:

* [ ] AWS account created
* [ ] Root MFA enabled
* [ ] IAM administrator user created
* [ ] Billing budget configured
* [ ] AWS CLI installed
* [ ] AWS CLI authenticated successfully

---

## Cleanup

No cleanup required.

These resources should remain available throughout the rest of the guide.

---

## CLF-C02 Concepts Reinforced

* Shared Responsibility Model
* Root User Protection
* Multi-Factor Authentication (MFA)
* IAM Users
* IAM Permissions
* Cost Awareness
* AWS CLI
* Programmatic Access
