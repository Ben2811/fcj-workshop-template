---
title: "Worklog Tuần 1"
date: 2026-07-05
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---


### Mục tiêu tuần 1:

* Thiết lập và bảo mật tài khoản AWS cá nhân, hiểu về IAM Users, Groups, Roles và cách switch role.
* Học cách quản lý và dự báo chi phí AWS với Budgets, tìm hiểu về các gói AWS Support Plans.
* Thiết kế và triển khai một custom VPC (public/private subnet, routing, NAT, VPN) và giám sát bằng Flow Logs & CloudWatch.
* Làm quen với nền tảng compute trên AWS: EC2 instance types, AMI, EBS và instance store.
* Tạo và thiết lập tài khoản AWS cá nhân, tìm hiểu các nguồn credit miễn phí và tiết kiệm chi phí.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ | --------------- | -------------- |
| 6   | - Tạo tài khoản AWS <br> - Hoàn thành 5 nhiệm vụ "Money-Making" để nhận credit <br> - Đọc danh sách Credit "Killer" <br> - Đọc các kiến trúc mẫu cho gói credit $200 <br> - Thiết lập billing alert và budget <br> - Khám phá AWS Console                                                        | 17/04/2026   | 17/04/2026      | https://000001.awsstudygroup.com/ |
| 2   | - Tìm hiểu AWS Identity and Access Management (IAM) access control <br> - Tạo IAM Group & IAM User <br> - Tạo IAM Role & IAM User <br> - Thực hành switch role                                                                                                                                  | 20/04/2026   | 20/04/2026      | https://000002.awsstudygroup.com/ |
| 3   | - Tìm hiểu quản lý chi phí AWS với Budgets: <br>&emsp; + Tạo Cost Budget <br>&emsp; + Tạo Usage Budget <br>&emsp; + Tạo Reserved Instance (RI) Budget <br>&emsp; + Tạo Savings Plans Budget                                                                                                     | 21/04/2026   | 21/04/2026      | https://000007.awsstudygroup.com/ |
| 4   | - Tìm hiểu về AWS Support Plans <br> - Đọc các loại Support Request <br> - Tạo Support Request <br> - Tìm hiểu cách đổi gói support                                                                                                                                                              | 22/04/2026   | 22/04/2026      | https://000009.awsstudygroup.com/ |
| 5   | - Tìm hiểu AWS VPC: <br>&emsp; + Thiết kế và triển khai custom VPC với public và private subnet <br>&emsp; + Cấu hình Route Table, Internet Gateway và NAT Gateway <br>&emsp; + Thiết lập VPC Flow Logs và CloudWatch metrics để giám sát network <br>&emsp; + Cấu hình Site-to-Site VPN (Customer Gateway & Virtual Private Gateway) | 23/04/2026   | 23/04/2026      | https://000003.awsstudygroup.com/ |
| 6   | - Tìm hiểu Compute (VM) trên AWS: <br>&emsp; + Instance types <br>&emsp; + AMI / Backup / Key Pair <br>&emsp; + Elastic Block Store (EBS) <br>&emsp; + Instance store                                                                                                                            | 24/04/2026   | 24/04/2026      |                 |


### Kết quả đạt được tuần 1:

* Tạo tài khoản AWS và hoàn thành thiết lập ban đầu: nhận credit miễn phí, xem qua các kiến trúc mẫu $200, thiết lập billing alert và budget, khám phá AWS Console.
* Tìm hiểu IAM access control và thực hành tạo IAM group, user, role, bao gồm cả việc switch giữa các role.
* Học cách quản lý và dự báo chi phí AWS bằng Cost, Usage, RI và Savings Plans Budget.
* Tìm hiểu về AWS Support Plans và cách tạo, quản lý Support Request.
* Thiết kế và triển khai custom VPC với public và private subnet, cấu hình Route Table, Internet Gateway và NAT Gateway để quản lý luồng traffic.
* Thiết lập VPC Flow Logs và CloudWatch metrics để giám sát hiệu năng network.
* Cấu hình các thành phần AWS Site-to-Site VPN (Customer Gateway & Virtual Private Gateway) để mô phỏng kết nối hybrid cloud.
* Làm quen với nền tảng compute trên AWS: instance types, AMI/Backup/Key Pair, EBS và instance store.

**Khó khăn & Giải pháp:**

* **Khó khăn:** Cấu hình sai (manual misconfiguration) trong quá trình thiết lập VPC.
* **Giải pháp:** Kiểm tra kỹ lại kiến trúc bằng VPC Resource Map.

**Dịch vụ AWS đã học trong tuần:** Amazon S3, Amazon EC2, IAM (Users, Groups, Roles), AWS Budgets, AWS Support, Amazon VPC (Subnet, Route Table, IGW, NAT Gateway, Flow Logs, Site-to-Site VPN), Amazon CloudWatch.


