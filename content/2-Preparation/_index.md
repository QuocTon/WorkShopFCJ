---
title : "Preparation "
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

## **2. Chuẩn bị**

Trước khi bắt đầu lab, hãy đảm bảo bạn đã có đầy đủ các điều kiện và công cụ cần thiết sau:  

### **Yêu cầu về tài khoản**
- Tài khoản **AWS** đã được tạo và **có quyền truy cập** các dịch vụ:
  - **Amazon S3**
  - **AWS Lambda**
  - **Amazon Macie**
  - **Amazon CloudWatch**
- Đã đăng nhập được vào **AWS Management Console**.

### **Kiến thức nền tảng**
- Hiểu cơ bản về giao diện **AWS Console**.
- Kiến thức cơ bản về **Python** hoặc **Node.js** (để viết Lambda function).

### **Công cụ hỗ trợ**
- **Trình duyệt web**: Chrome hoặc Edge (phiên bản mới nhất).
- **VSCode** hoặc trình soạn thảo code khác (nếu viết Lambda code local).
- **JSON Editor** hoặc plugin hỗ trợ định dạng JSON (dùng để tạo test event cho Lambda).

### **Dữ liệu mẫu**
- **File CSV** chứa dữ liệu nhạy cảm giả lập (ví dụ: _email_, _số điện thoại_).
  - Ví dụ cấu trúc file:
    ```csv
    name,email,phone
    Nguyen Van A,examplea@gmail.com,0901234567
    Tran Thi B,exampleb@yahoo.com,0912345678
    ```

> 💡 **Mẹo:** Bạn có thể tạo file CSV thủ công bằng Excel hoặc Google Sheets, sau đó lưu dưới định dạng `.csv` để upload lên Amazon S3.
