---
title : "Prerequiste"
date : 2024-01-01
weight : 2
chapter : false
pre : " <b> 5.2. </b> "
---

#### Install and configure the AWS CLI

This whole Admin Panel & Data (Chuong Tu Luan) section is done with the AWS CLI v2. Check that it's installed:

```bash
aws --version
```

![aws --version](/images/5-Workshop/5.2-Prerequiste/01-version.png)

Configure your credentials and default region (the same `ap-southeast-1` PeriodIQ runs in):

```bash
aws configure
```

Verify the credentials are working:

```bash
aws sts get-caller-identity
```

![aws sts get-caller-identity](/images/5-Workshop/5.2-Prerequiste/02-identity.png)

> **CLI Note:** `aws sts get-caller-identity` is the fastest way to confirm the CLI is authenticated correctly and to grab your Account ID before running anything else.

#### Required IAM permissions

As Chuong Tu Luan, my IAM user needs permissions for the services I own: `dynamodb`, `lambda`, `apigateway`, `cognito-idp`, plus `iam` and `s3` (for the Admin Panel frontend build/deploy). For a personal/sandbox account, attaching the AWS managed `AdministratorAccess` policy is the simplest option.

> **CLI Note:** every step on this page - version check, configure, identity check - is itself a CLI command. Sections 5.6.1-5.6.3 that follow are the same: every action goes through the CLI, and the console (plus the admin dashboard) only gets opened afterward to cross-check the evidence, not to perform the actions themselves.
