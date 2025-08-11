---
title: "Xem log Lambda"
date: "2025-08-10"
weight: 1
chapter: false
pre: "<b> 6.1 </b>"
---

### 6.1. Xem log Lambda {#xem-log-lambda}

1. **Truy cập CloudWatch Logs**  
   - Đăng nhập vào [AWS Console](https://console.aws.amazon.com/).  
   - Tìm kiếm và chọn **CloudWatch**.

   ![Trang chính CloudWatch](/images/6.cloudwatch/cloudwatch-dashboard.png)

2. **Mở log group của Lambda**  
   - Trong sidebar trái, chọn **Logs > Log groups**.  
   - Tìm log group của Lambda, ví dụ: `/aws/lambda/masking-function`.  
   - Chọn log stream mới nhất.

   ![Log group Lambda](/images/6.cloudwatch/log-group.png)

3. **Xem dữ liệu log**  
   - Tìm dòng log chứa:
     ```
     Masked: ****er123@gmail.com
     ```

   ![Dữ liệu log Lambda](/images/6.cloudwatch/lambda-log-data.png)
