---
title : "Giới thiệu"
date : 2024-01-01
weight : 1
chapter : false
pre : " <b> 5.1. </b> "
---

#### PeriodIQ là gì?

PeriodIQ là một ứng dụng serverless sinh giáo án tập gym cá nhân hoá trong 4 tuần dựa trên trình độ, cân nặng, mục tiêu tập luyện và Personal Record của người dùng, thông qua một rule engine (Volume Filter -> Conflict Resolution -> Progression Builder). Toàn bộ kiến trúc (16 dịch vụ AWS trải trên 8 tầng) được mô tả ở phần [Proposal](../../2-proposal/).

#### Team đã chia công việc như thế nào

| Mục | Vai trò | Dịch vụ AWS |
|---|---|---|
| Lê Hoài Huân | Auth & User Profile | Amazon Cognito, AWS WAF, Amazon CloudFront |
| Trần Anh Tài | Rule Engine & Sinh giáo án | Lambda (API Handler + Rule Engine), Amazon S3 |
| Lê Hữu Duy Hoàng | Tiến trình & Async Notification | Amazon SQS, Lambda Worker, Amazon SNS |
| **Chương Tử Luân (tôi)** | **Admin Panel & Data** | **Lambda Admin API, Amazon DynamoDB, API Gateway** |
| Phạm Văn Sỹ | CI/CD & Monitoring | AWS CodePipeline, AWS CodeBuild, CloudFormation/SAM, Amazon CloudWatch |

#### Phạm vi của workshop này

Workshop này ghi lại chi tiết **vai trò của chính tôi, Chương Tử Luân**, dùng **đúng dữ liệu và hạ tầng production đang chạy** - không phải bản dựng lại rút gọn. 8 bảng DynamoDB (định nghĩa trong `template.yml`), Lambda Admin API đọc/ghi các bảng đó, và Admin Panel frontend xây trên cả hai đều là resource đã deploy sẵn trong chính account AWS mà project này đang chạy. Mọi lệnh ở [mục 5.6](../5.6-nguoi4-admin/) đều là lệnh `aws` CLI gọi trực tiếp trên deployment đó - đọc bảng thật, GSI thật, số lượng record thật, và hành vi API/frontend thật - kèm ảnh chụp terminal hoặc trình duyệt làm bằng chứng cho từng bước.

> **CLI Note:** vì workshop này ghi lại hệ thống production đang sống thay vì một bản sao sandbox dùng-rồi-bỏ, mọi thứ ở đây đều **chỉ đọc** - `describe-table`, `list-tables`, `scan`. Không có gì bị tạo, thay đổi, hay xoá trên hạ tầng trong lúc viết phần này (xem [Dọn dẹp tài nguyên](../5.8-cleanup/) để biết điều đó có nghĩa gì trong thực tế).
