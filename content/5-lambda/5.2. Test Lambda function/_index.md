---
title: "Test Lambda function"
date: "2025-08-10"
weight: 2
chapter: false
pre: "<b> 5.2 </b>"
---

### 5.2. Test Lambda function {#test-lambda}

1. **Tạo event test**  
   - Trong tab **Test**, chọn **Configure test event**.  
   - Đặt tên event: `eventtestlambda`.  
   - Dán nội dung JSON:
     ```json
     {
       "email": "exampleuser123@gmail.com"
     }
     ```
   - Nhấn **Save**.

   ![Tạo event test Lambda](/images/5.lambda/create-test-event.png)

2. **Chạy test**  
   - Nhấn **Test** để chạy hàm.  
   - Kết quả trả về:
     ```json
     {
       "masked_email": "****er123@gmail.com"
     }
     ```

   ![Kết quả test Lambda](/images/5.lambda/lambda-test-result.png)

---

> 📌 **Mẹo**: Kỹ thuật này có thể áp dụng cho nhiều loại dữ liệu nhạy cảm khác như số thẻ ngân hàng, số CMND/CCCD…
