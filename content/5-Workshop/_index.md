---
title: "Workshop"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

# Deploying PeriodIQ Using the AWS CLI - By Team Role

#### Overview

**PeriodIQ** is a serverless "automatic personal trainer" built by a 5-person team, each owning 3-4 AWS services (see the [Proposal](../2-proposal/)). This section is organized to mirror that same team structure - one part per person. For this report, I only document my own role in detail: **Chuong Tu Luan (Admin Panel & Data)**, covering **Amazon DynamoDB, the Lambda Admin API, and API Gateway**, plus the **Admin Panel frontend** built on top of them - every step done with the **AWS CLI** and verified with a real screenshot.

#### Content

1. [Workshop overview](5.1-Workshop-overview/)
2. [Prerequisites](5.2-Prerequiste/)
3. [Le Hoai Huan - Auth & User Profile](5.3-Nguoi1-Auth/)
4. [Tran Anh Tai - Rule Engine & Workout Generation](5.4-Nguoi2-RuleEngine/)
5. [Le Huu Duy Hoang - Progress & Async Notification](5.5-Nguoi3-Async/)
6. [Chuong Tu Luan - Admin Panel & Data](5.6-Nguoi4-Admin/) *(my role - documented in detail below)*
7. [Pham Van Sy - CI/CD & Monitoring](5.7-Nguoi5-CICD/) *(a teammate's role - included for context)*
8. [Clean up](5.8-Cleanup/)
