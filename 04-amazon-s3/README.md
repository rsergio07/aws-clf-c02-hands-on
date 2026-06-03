# 04 - Amazon S3

## Objective

Learn the fundamentals of Amazon Simple Storage Service (Amazon S3), one of the most frequently referenced services in the AWS Certified Cloud Practitioner (CLF-C02) exam.

By the end of this module, you will be able to:

* Create an S3 bucket
* Upload and download objects
* Enable versioning
* Understand storage classes
* Configure lifecycle policies
* Use S3 through both the AWS Console and AWS CLI

Estimated time: 30-45 minutes

---

## Why S3 Matters

Amazon S3 is AWS's object storage service.

Many AWS services use S3 directly or indirectly.

Common use cases include:

* File storage
* Static website hosting
* Application assets
* Backups
* Log storage
* Data lakes

S3 is highly durable, scalable, and managed by AWS.

---

## Key Concepts

### Bucket

A bucket is a container for storing objects.

Example:

```text id="4s55e4"
my-clf-practice-bucket
```

Bucket names must be globally unique.

---

### Object

An object is a file stored in a bucket.

Examples:

```text id="yl14t3"
image.jpg
report.pdf
notes.txt
```

Each object consists of:

* Data
* Metadata
* Key (object name)

---

### Storage Classes

Common storage classes:

* S3 Standard
* S3 Standard-IA
* S3 One Zone-IA
* S3 Glacier Instant Retrieval
* S3 Glacier Flexible Retrieval
* S3 Glacier Deep Archive

For CLF-C02, focus on understanding when each is used.

---

### Versioning

Versioning allows multiple versions of the same object to exist.

Benefits:

* Accidental deletion recovery
* Rollback capability
* Change tracking

---

### Lifecycle Policies

Lifecycle policies automatically move or delete objects based on age.

Example:

```text id="k5x6eu"
Move to Glacier after 30 days
Delete after 365 days
```

---

## Activity 1 - Create a Bucket

Using the AWS Console:

1. Open Amazon S3
2. Create a bucket
3. Choose a globally unique name
4. Accept default settings

Expected result:

* One S3 bucket created

---

## Activity 2 - Upload Objects

Upload:

```text id="hy61h0"
sample.txt
image.png
```

Review:

* Object names
* Object size
* Last modified date

Expected result:

* Objects stored successfully

---

## Activity 3 - Download Objects

Download a previously uploaded object.

Expected result:

* Object retrieved successfully

---

## Activity 4 - Enable Versioning

Open:

```text id="c7q9e3"
Bucket
→ Properties
→ Bucket Versioning
```

Enable versioning.

Modify and upload the same file again.

Observe:

* Multiple object versions

Expected result:

* Version history visible

---

## Activity 5 - Review Storage Classes

Open object properties.

Review available storage classes.

Understand typical use cases for:

* Standard
* Standard-IA
* Glacier

Expected result:

* Familiarity with storage tiers

---

## Activity 6 - Create a Lifecycle Rule

Create a lifecycle policy.

Example:

```text id="8fmxui"
Transition objects after 30 days
```

Review the configuration.

Expected result:

* Lifecycle rule configured

---

## Activity 7 - Use AWS CLI

List buckets:

```bash id="g2b5kp"
aws s3 ls
```

List bucket contents:

```bash id="z8kz0l"
aws s3 ls s3://YOUR-BUCKET-NAME
```

Upload a file:

```bash id="pk0a7o"
aws s3 cp sample.txt s3://YOUR-BUCKET-NAME
```

Download a file:

```bash id="5i8w4d"
aws s3 cp s3://YOUR-BUCKET-NAME/sample.txt .
```

Expected result:

* Successful upload and download using AWS CLI

---

## Console vs CLI

Use the Console when:

* Learning S3
* Exploring bucket settings
* Managing lifecycle policies

Use the CLI when:

* Automating uploads
* Managing large numbers of objects
* Building scripts

---

## Cleanup

Delete:

* Uploaded objects
* Lifecycle rules (optional)
* Test bucket

Delete bucket:

```bash id="l31gm8"
aws s3 rb s3://YOUR-BUCKET-NAME --force
```

Expected result:

* No unnecessary S3 resources remain

---

## CLF-C02 Concepts Reinforced

* Object Storage
* Buckets
* Objects
* Versioning
* Storage Classes
* Lifecycle Policies
* Durability
* Scalability
* AWS CLI
* Cost Optimization
