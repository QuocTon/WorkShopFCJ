---
title : "Introduction"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
Trong thời đại số, dữ liệu được xem là tài sản quan trọng của mỗi tổ chức, đặc biệt là dữ liệu nhạy cảm như thông tin cá nhân, _email_, _số điện thoại_ hoặc thông tin tài chính. Việc bảo vệ dữ liệu này không chỉ đáp ứng yêu cầu pháp lý (ví dụ: **GDPR**, **HIPAA**) mà còn giúp duy trì uy tín và niềm tin của khách hàng.  

Lab này được thiết kế nhằm giúp bạn tiếp cận và thực hành trực tiếp các dịch vụ bảo mật của AWS để quản lý vòng đời dữ liệu nhạy cảm — từ **lưu trữ**, **nhận diện**, **che giấu**, cho đến **giám sát**. Cụ thể, bạn sẽ được hướng dẫn:  

- **Amazon S3** – Lưu trữ và quản lý dữ liệu an toàn, thiết lập quyền truy cập phù hợp.  
- **Amazon Macie** – Phát hiện tự động các thông tin nhạy cảm trong dữ liệu lưu trữ.  
- **AWS Lambda** – Xây dựng chức năng che giấu (_mask_) thông tin, đảm bảo dữ liệu không bị lộ khi xử lý.  
- **Amazon CloudWatch** – Giám sát hoạt động của Lambda và tạo cảnh báo khi có sự kiện đặc biệt.  

> 💡 **Kết quả mong đợi:**  
> Sau khi hoàn thành lab này, bạn sẽ:  
> - Thành thạo các thao tác cơ bản với **S3**, **Macie**, **Lambda** và **CloudWatch**.  
> - Biết cách áp dụng kỹ thuật _masking_ để bảo vệ thông tin nhạy cảm.  
> - Nắm quy trình **dọn dẹp tài nguyên** để tránh phát sinh chi phí không cần thiết.