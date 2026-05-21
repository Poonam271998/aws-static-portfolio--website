# aws-static-portfolio--website
# ☁️ AWS Static Portfolio Website with CloudFront, Monitoring & Security

A complete AWS Cloud Practitioner capstone project demonstrating how to deploy, secure, monitor, and manage a static portfolio website using core AWS services.

This project simulates a real-world cloud deployment that a junior cloud engineer or cloud support associate might implement for a client or organization.

---

# 📌 Project Overview

This project focuses on hosting a static website on AWS while implementing security, monitoring, auditing, and billing protection best practices.

The website is hosted using Amazon S3 and distributed globally through Amazon CloudFront for improved performance and HTTPS security.

Additional AWS services such as IAM, CloudWatch, CloudTrail, SNS, AWS Budgets, and Trusted Advisor are integrated to create a secure and production-ready cloud environment.

---

# 🧰 AWS Services Used

| AWS Service | Purpose |
|---|---|
| Amazon S3 | Static website hosting |
| Amazon CloudFront | CDN and HTTPS delivery |
| AWS IAM | Identity and access management |
| Amazon CloudWatch | Monitoring and alarms |
| AWS CloudTrail | Audit logging |
| Amazon SNS | Email notifications |
| AWS Budgets | Billing alerts |
| AWS Trusted Advisor | Security and optimization checks |

---

# 🏗️ Architecture Diagram

```text
                    User Browser
                          │
                          ▼
                 Amazon CloudFront
                          │
                          ▼
                    Amazon S3 Bucket
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
 CloudWatch          CloudTrail         AWS Budgets
 Monitoring           Audit Logs         Cost Alerts
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                    Amazon SNS
                  Email Notifications
