# 02 - IAM (Identity and Access Management)

## Objective

Learn how AWS controls access to services and resources using IAM.

By the end of this module, you will be able to:

* Create IAM users
* Create IAM groups
* Assign permissions using policies
* Understand least privilege
* Differentiate authentication from authorization

Estimated time: 20-30 minutes

---

## Why IAM Matters

IAM is one of the most important AWS services.

Almost every AWS action depends on IAM permissions.

Examples:

* Can a user launch an EC2 instance?
* Can a user create an S3 bucket?
* Can a user view billing information?
* Can a user delete resources?

IAM determines the answer.

---

## Key Concepts

### Authentication

Authentication answers:

```text id="cjlwmz"
Who are you?
```

Examples:

* Username and password
* Access keys
* MFA

---

### Authorization

Authorization answers:

```text id="s5s8sj"
What are you allowed to do?
```

Examples:

* Read-only access
* Administrator access
* S3-only access

---

### IAM User

Represents an individual identity.

Examples:

```text id="gl1ujf"
alice
bob
developer01
```

Users can:

* Sign in to the AWS Console
* Use AWS CLI
* Use AWS SDKs

---

### IAM Group

A collection of users.

Examples:

```text id="w1o9qg"
Administrators
Developers
Auditors
```

Permissions are usually assigned to groups instead of individual users.

---

### IAM Policy

A document that defines permissions.

Policies answer:

```text id="eym1i0"
Allow or deny which actions?
On which resources?
```

---

## Activity 1 - Explore AWS Managed Policies

Open:

```text id="b4ezq0"
IAM
→ Policies
```

Search for:

```text id="l74thj"
AdministratorAccess
ReadOnlyAccess
AmazonS3ReadOnlyAccess
AmazonEC2ReadOnlyAccess
```

Observe:

* Policy names
* Permission scope
* AWS managed policies

Expected result:

* Familiarity with common AWS policies

---

## Activity 2 - Create a Read-Only User

Create a user:

```text id="3sn5tb"
readonly-user
```

Assign:

```text id="zwh4i8"
ReadOnlyAccess
```

Test:

* User can view resources
* User cannot create resources

Expected result:

* Understand permission boundaries

---

## Activity 3 - Create a Custom Group

Create:

```text id="r2b3za"
S3-Readers
```

Attach:

```text id="t0i6xm"
AmazonS3ReadOnlyAccess
```

Expected result:

* Understand group-based permission management

---

## Activity 4 - Review Existing Users

Using AWS Console:

```text id="n3o9x7"
IAM
→ Users
```

Review:

* Console access
* MFA status
* Assigned permissions

Expected result:

* Better understanding of account security posture

---

## Activity 5 - Explore IAM with AWS CLI

List users:

```bash id="omgk53"
aws iam list-users
```

List groups:

```bash id="kk9z7m"
aws iam list-groups
```

List policies:

```bash id="v3p80m"
aws iam list-policies --scope AWS
```

Expected result:

* Understand how IAM resources can be inspected programmatically

---

## Security Best Practices

* Enable MFA for privileged users
* Avoid using the root account
* Assign permissions to groups
* Follow least privilege
* Rotate access keys when necessary

---

## Cleanup

Remove any temporary test users created during this module.

Keep:

* Administrative IAM user
* MFA configuration
* IAM groups used in later modules

---

## CLF-C02 Concepts Reinforced

* IAM Users
* IAM Groups
* IAM Policies
* Authentication
* Authorization
* Least Privilege
* Multi-Factor Authentication (MFA)
* Shared Responsibility Model
* AWS Managed Policies
