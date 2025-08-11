---
title: "Tạo bucket trên Amazon S3"
date: "2025-08-10"
weight: 1
chapter: false
pre: "<b> 3.1 </b>"
---

### 3.1. Tạo bucket trên S3 {#tao-bucket-s3}

1. **Truy cập AWS Management Console**  
   - Đăng nhập vào [AWS Console](https://console.aws.amazon.com/).  
   - Tìm dịch vụ **S3** trong thanh tìm kiếm và chọn **Amazon S3**.

   ![Trang chính Amazon S3](/images/1.s3/001-s3.png)

2. **Tạo bucket mới**  
   - Nhấn **Create bucket**.  
   - **Bucket name**: đặt tên duy nhất trên toàn hệ thống AWS (ví dụ: `lab-privacy-demo-12345`).  
   - **AWS Region**: chọn cùng region với các dịch vụ khác (ví dụ: `ap-southeast-1` – Singapore).  
   - **Block Public Access settings**: giữ nguyên mặc định (bật tất cả) để bảo mật.  
   - Nhấn **Create bucket**.

   ![Giao diện tạo bucket S3](/images/1.s3/create-bucket.png)
