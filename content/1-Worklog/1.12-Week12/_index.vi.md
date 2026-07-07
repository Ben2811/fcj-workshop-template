---
title: "Worklog Tuần 12"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.12 </b> "
---

### Mục tiêu tuần 12:

* Kiểm tra và xác thực frontend Admin Panel đã xây dựng ở tuần 11 với Lambda Admin API và dữ liệu DynamoDB thật.
* Bắt đầu viết chương AWS Workshop tài liệu hóa toàn bộ dự án PeriodIQ đã hoàn thành, sử dụng hạ tầng thật đã triển khai làm bằng chứng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------- |
| 2   | - Kiểm tra frontend Admin Panel end-to-end với Admin API và dữ liệu DynamoDB thật (trang Dashboard, Exercises, Rules, Templates) <br> - Sửa các lỗi phát hiện được trong quá trình rà soát | 06/07/2026   | 06/07/2026      | <https://github.com/PeriolIQ/PeriodIQ> |
| 3   | - Bắt đầu viết phần tổng quan và phần chuẩn bị của AWS Workshop                                                                                       | 07/07/2026   | 07/07/2026      | <https://github.com/Ben2811/fcj-workshop-template> |
| 4   | - Viết mục 5.6 của AWS Workshop (Admin Panel & Data): DynamoDB, Lambda Admin API, frontend Admin Panel, kèm bằng chứng CLI/screenshot thật             | 08/07/2026   | 08/07/2026      | <https://github.com/Ben2811/fcj-workshop-template> |
| 5   | - Viết các phần của Workshop tài liệu hóa vai trò của các đồng đội (Auth & User Profile, Rule Engine & Workout Generation, Progress & Async Notification, CI/CD & Monitoring) | 09/07/2026   | 09/07/2026      | <https://github.com/Ben2811/fcj-workshop-template> |
| 6   | - Rà soát và đồng bộ nội dung Workshop giữa bản tiếng Anh và tiếng Việt                                                                                | 10/07/2026   | 10/07/2026      | <https://github.com/Ben2811/fcj-workshop-template> |


### Kết quả đạt được tuần 12:

* Kiểm tra frontend Admin Panel bằng React end-to-end với Lambda Admin API và dữ liệu DynamoDB thật, và sửa các lỗi phát hiện được trong quá trình rà soát.

* Bắt đầu và có tiến triển tốt với chương AWS Workshop cho bài báo cáo thực tập, bao gồm:
  * Phần tổng quan workshop và phần chuẩn bị.
  * Phần của riêng tôi (5.6 - Admin Panel & Data), có bằng chứng là các lệnh `aws` CLI và screenshot thật chạy trên hệ thống đang triển khai, không phải bản dựng lại đơn giản hóa.
  * Các phần tài liệu hóa vai trò của đồng đội (Auth & User Profile, Rule Engine & Workout Generation, Progress & Async Notification, CI/CD & Monitoring), đồng bộ giữa bản tiếng Anh và tiếng Việt.

* Rèn luyện kỹ năng chuyển hóa một dự án serverless thật, đã triển khai thành tài liệu dạng workshop mà kỹ sư khác có thể theo dõi và kiểm chứng từng bước.

**Dịch vụ AWS đã sử dụng trong tuần:** Amazon DynamoDB, AWS Lambda, Amazon API Gateway.

