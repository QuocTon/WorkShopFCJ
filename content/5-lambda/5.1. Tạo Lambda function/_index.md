---
title: "Tạo Lambda function"
date: "2025-08-10"
weight: 1
chapter: false
pre: "<b> 5.1 </b>"
---

### 5.1. Tạo Lambda function {#tao-lambda}

1. **Truy cập AWS Console**  
   - Đăng nhập vào [AWS Console](https://console.aws.amazon.com/).  
   - Tìm kiếm và chọn **Lambda**.

   ![Trang chính AWS Lambda](/images/5.lambda/lambda-dashboard.png)

2. **Tạo function mới**  
   - Chọn **Create function**.  
   - **Author from scratch**.  
   - **Function name**: `masking-function`.  
   - **Runtime**: Python 3.12.  
   - Nhấn **Create function**.

   ![Tạo Lambda function](/images/5.lambda/create-lambda.png)

3. **Thêm mã Python**  
   - Trong phần **Code source**, xóa nội dung mặc định và dán đoạn mã sau:
     ```python
     def lambda_handler(event, context):
         email = event.get("email", "unknown@example.com")
         masked = "****" + email[-10:]
         print("Masked:", masked)
         return {
             "masked_email": masked
         }
     ```
   - Nhấn **Deploy** để lưu.

   ![Code Lambda che dấu dữ liệu](/images/5.lambda/code-lambda.png)
