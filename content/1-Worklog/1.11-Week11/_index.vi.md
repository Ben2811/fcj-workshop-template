---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---



### Mục tiêu tuần 11:

* Triển khai authentication, SSL và messaging (SQS/SNS) cho ứng dụng serverless.
* Tự động hoá CI/CD và bổ sung khả năng giám sát (CloudWatch & X-Ray) cho ứng dụng serverless.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                       | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | -------------------------------------------------------------------------------- | ------------ | --------------- | -------------- |
| 2   | - **PeriodIQ:** tạo 8 bảng DynamoDB cùng các GSI trên hạ tầng triển khai thật                    | 29/06/2026   | 29/06/2026      |  <https://github.com/PeriolIQ/PeriodIQ>  |
| 3   | - **PeriodIQ:** xây dựng các controller của Lambda Admin API phía sau API Gateway                | 30/06/2026   | 30/06/2026      |  <https://github.com/PeriolIQ/PeriodIQ>  |
| 4   | - **PeriodIQ:** viết unit test cho các controller của Lambda Admin API                            | 01/07/2026   | 01/07/2026      |  <https://github.com/PeriolIQ/PeriodIQ>  |
| 5   | - **PeriodIQ:** xây dựng frontend Admin Panel bằng React (Dashboard, Exercises, Rules, Templates) | 02/07/2026   | 02/07/2026      |  <https://github.com/PeriolIQ/PeriodIQ>  |
| 6   | - **PeriodIQ:** kết nối frontend Admin Panel với Admin API và kiểm tra end-to-end                 | 03/07/2026   | 03/07/2026      |  <https://github.com/PeriolIQ/PeriodIQ>  |

### Kết quả đạt được tuần 11:

* Triển khai authentication cho ứng dụng serverless bằng Amazon Cognito.
* Thiết lập SSL/TLS cho ứng dụng serverless.
* Xây dựng workflow xử lý đơn hàng bằng Amazon SQS và SNS.
* Tự động hoá CI/CD cho ứng dụng serverless bằng AWS CodePipeline.
* Giám sát ứng dụng serverless bằng Amazon CloudWatch và AWS X-Ray.
* **Dự án thực hành PeriodIQ:** tạo 8 bảng DynamoDB cùng GSI, xây dựng các controller của Lambda Admin API kèm unit test, và xây dựng frontend Admin Panel bằng React — hoàn thành vai trò Admin Panel & Data từ đầu đến cuối.

**Dịch vụ AWS đã học trong tuần:** AWS SAM, Amazon Cognito, Amazon SQS, Amazon SNS, AWS CodePipeline, Amazon CloudWatch, AWS X-Ray.


