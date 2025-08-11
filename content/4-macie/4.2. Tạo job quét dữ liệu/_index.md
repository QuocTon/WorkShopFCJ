---
title: "Tạo job quét dữ liệu với Macie"
date: "2025-08-10"
weight: 2
chapter: false
pre: "<b> 4.2 </b>"
---

### 4.2. Tạo job quét dữ liệu {#tao-job-quet}

1. **Tạo job quét**  
   - Trong Amazon Macie, vào **Jobs** → **Create Job**.  
   - Chọn bucket S3 chứa file `sample.csv`.

   ![Chọn bucket để quét dữ liệu](/images/4.macie/select-bucket.png)

2. **Cấu hình job**  
   - Chọn **One-time** hoặc **Scheduled** (định kỳ).  
   - Chọn **Managed data identifiers**: Email address, Phone number, v.v.  
   - Giữ nguyên các tùy chọn khác.

   ![Cấu hình job quét dữ liệu](/images/4.macie/configure-job.png)

3. **Xem kết quả quét**  
   - Sau khi chạy xong, vào tab **Findings** để xem dữ liệu nhạy cảm phát hiện được.

   ![Kết quả phát hiện dữ liệu nhạy cảm](/images/4.macie/macie-findings.png)
