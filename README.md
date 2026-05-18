# AWS S3 Public Web Hosting & Object ACL Challenge

A hands-on cloud infrastructure project demonstrating secure object-level access control, bucket permission management, and static web hosting automation using the AWS CLI and AWS Management Console.

---

## Project Objectives
* **Infrastructure Provisioning**: Deployed a globally unique Amazon S3 bucket within the `us-west-2` (Oregon) region.
* **Security & Access Control**: Modified bucket-level **Block Public Access** settings to safely allow specific public interactions.
* **Object Ownership Tuning**: Updated **Object Ownership Controls** to activate and restore legacy Access Control Lists (ACLs) using `BucketOwnerPreferred`.
* **Granular Permissions**: Applied fine-grained `public-read` ACL rules strictly to individual objects (`index.html`) rather than opening up the entire bucket infrastructure.
* **Verification**: Verified global browser routing and programmatic resource tracking via the AWS CLI.

---

## Tech Stack & Tools
* **Cloud Provider**: Amazon Web Services (AWS)
* **Core Service**: Amazon S3 (Simple Storage Service)
* **Interface**: AWS Command Line Interface (CLI) via EC2 CLI Host
* **Languages**: HTML, Bash / Linux Shell

---

## Step-by-Step Implementation

### 1. Environment Initialization
Configured the AWS CLI client with runtime lab credentials, designating JSON output routing and regional targets:
```bash
aws configure
