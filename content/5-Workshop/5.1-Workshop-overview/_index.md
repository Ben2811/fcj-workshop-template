---
title : "Introduction"
date : 2024-01-01
weight : 1
chapter : false
pre : " <b> 5.1. </b> "
---

#### What is PeriodIQ?

PeriodIQ is a serverless application that generates a personalized 4-week gym workout plan for a user based on their fitness level, body weight, training goal, and Personal Records, using a rule-based engine (Volume Filter -> Conflict Resolution -> Progression Builder). The full architecture (16 AWS services across 8 layers) is described in the [Proposal](../../2-proposal/) section.

#### How the team split the work

| Section | Role | AWS Services |
|---|---|---|
| Le Hoai Huan | Auth & User Profile | Amazon Cognito, AWS WAF, Amazon CloudFront |
| Tran Anh Tai | Rule Engine & Workout Generation | Lambda (API Handler + Rule Engine), Amazon S3 |
| Le Huu Duy Hoang | Progress & Async Notification | Amazon SQS, Lambda Worker, Amazon SNS |
| **Chuong Tu Luan (me)** | **Admin Panel & Data** | **Lambda Admin API, Amazon DynamoDB, API Gateway** |
| Pham Van Sy | CI/CD & Monitoring | AWS CodePipeline, AWS CodeBuild, CloudFormation/SAM, Amazon CloudWatch |

#### Scope of this workshop

This workshop documents **my own role, Chuong Tu Luan**, in detail, using the **actual production data and infrastructure** - not a simplified rebuild. The 8 DynamoDB tables (defined in the real `template.yml`), the Lambda Admin API that reads and writes them, and the Admin Panel frontend built on top of both are all real, already-deployed resources in the AWS account this project runs in. Every command in [section 5.6](../5.6-nguoi4-admin/) is a genuine `aws` CLI call against that real deployment - reading real tables, real GSIs, real record counts, and real API/frontend behavior - with a real terminal or browser screenshot as evidence for each one.

> **CLI Note:** because this workshop documents the live production system rather than a disposable sandbox copy, everything here is **read-only** - `describe-table`, `list-tables`, `scan` - against the real DynamoDB tables. Nothing was created, changed, or deleted on the real infrastructure while writing this section (see [Clean up](../5.8-cleanup/) for what that means in practice).
