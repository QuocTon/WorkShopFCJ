---
title: "Tạo cảnh báo khi log match"
date: "2025-08-10"
weight: 2
chapter: false
pre: "<b> 6.2 </b>"
---

### 6.2. Tạo cảnh báo {#tao-canh-bao}

1. **Tạo Metric Filter**  
   - Trong log group của Lambda, nhấn **Actions > Create metric filter**.  
   - Ở **Filter pattern**, nhập:
     ```
     Masked:
     ```
   - Nhấn **Next**.

   ![Tạo metric filter](/images/6.cloudwatch/create-metric-filter.png)

2. **Cấu hình Metric Filter**  
   - **Filter name**: `MaskedFilter`.  
   - **Metric namespace**: `LambdaMonitor`.  
   - **Metric name**: `MaskedOutputFound`.  
   - **Metric value**: `1`.  
   - Nhấn **Create filter**.

   ![Cấu hình metric filter](/images/6.cloudwatch/configure-metric-filter.png)

3. **Kiểm tra kết quả**  
   - Chạy lại Lambda và xem log mới.  
   - Nếu log chứa `Masked:`, metric sẽ ghi nhận giá trị = 1.

   ![Kết quả filter match](/images/6.cloudwatch/filter-match-result.png)

---

> 📌 **Mẹo**: Có thể kết hợp Metric Filter với CloudWatch Alarm để gửi email cảnh báo qua SNS khi metric đạt giá trị nhất định.
