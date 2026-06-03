# IAM (Identity and Access Management)

## Purpose

AWS Identity and Access Management (IAM) allows you to securely control access to AWS services and resources.

IAM is one of the most important services for both the AWS Certified Cloud Practitioner (CLF-C02) exam and real-world AWS environments.

## CLF-C02 Concepts Covered

* AWS Shared Responsibility Model
* IAM Users
* IAM Groups
* IAM Policies
* Least Privilege
* Multi-Factor Authentication (MFA)
* Root User Protection
* Authentication vs Authorization

## Why IAM Matters

A common AWS security best practice is:

> Never use the root account for daily activities.

Instead:

1. Secure the root account.
2. Enable MFA.
3. Create IAM users.
4. Assign permissions using groups and policies.
5. Follow the principle of least privilege.

## Hands-On Activities

### Activity 1 – Review Account Security

Verify:

* Root account exists
* MFA is enabled
* Billing access is configured
* Recovery information is up to date

### Activity 2 – Create an Administrative IAM User

Create an IAM user for daily administration.

Recommended permissions:

* AdministratorAccess

Validate:

* Console login works
* AWS CLI authentication works

### Activity 3 – Create a Read-Only User

Create a second IAM user with:

* ReadOnlyAccess

Validate:

* Can view resources
* Cannot create resources

### Activity 4 – Explore IAM Policies

Review examples of:

* AWS Managed Policies
* Customer Managed Policies
* Inline Policies

Examples:

* AdministratorAccess
* ReadOnlyAccess
* AmazonS3ReadOnlyAccess

### Activity 5 – Enable MFA

Enable MFA for:

* Root user
* Administrative IAM user

## Useful AWS CLI Commands

Get current identity:

```bash
aws sts get-caller-identity
```

List IAM users:

```bash
aws iam list-users
```

List IAM groups:

```bash
aws iam list-groups
```

List IAM policies:

```bash
aws iam list-policies --scope AWS
```

## Cleanup

If this is a personal AWS account:

* Keep the administrative IAM user.
* Keep MFA enabled.
* Remove only temporary test users.

Do not remove:

* Root account MFA
* Security configurations
* Billing access settings

## Key Takeaways

* Root user should be protected and rarely used.
* IAM controls authentication and authorization.
* Policies define permissions.
* Groups simplify permission management.
* MFA is a critical security control.
* Least privilege reduces security risk.
