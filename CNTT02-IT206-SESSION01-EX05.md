
# Bài 5: Áp dụng AI Policy & Nguyên tắc Human-in-the-loop trong Đánh giá Nhân sự
## Cách AI đoán từ (bản chất LLM)
- Không Suy Luận như con người: AI là cỗ máy tính toán xác suất để đoán từ/ký tự (token) tiếp theo có khả năng xuất hiện cao nhất dựa trên dữ liệu đã học 
- Hệ quả: giỏi bắt chước mẫu code phổ biến nhưng không tự hiểu ngữ cảnh hệ thống của bạn luôn phải chạy thử và kiểm lại code 
## 2 Cách nhận diện "ảo giác "AI 
- bịa hàm/thư viện: tạo ra hàm nghe rất hợp lý nhưng không hề tồn tại khi biên dịch lỗi 
- Chém gió lỗi logic: không nhận mình sai với các bài toán khó, mà tự chế ra đoạn code tự chạy được nhưng không bug ngầm 
- tạo link/tài liệu ma: bịa ra đường dẫn tài liệu hoặc nguồn tham khảo báo lỗi 404 khi truy cập 
## Khung viết prompt chuẩn CREATE 
- [x] C (CONTEXT-BỐI CẢNH) bạn là ai, đang làm gì   
- [x] R (Role-vai trò) AI đóng vai trò VD Giảng viên hướng dẫn dễ tính
- [x] E (Explicit task nhiệm vụ) Làm chính xác việc gì? (VD: Giải thích vòng lặp for)      
- [x] A(Audience - Đối tượng): Viết cho ai đọc? (VD: Người mới bắt đầu học code)
- [X] T - Tone/Style (Giọng điệu/Phong cách): Trình bày thế nào?
- [X] E - Examples/Constraints (Ví dụ mẫu hoặc Ràng buộc): Giới hạn hoặc định dạng đầu ra.
```
Mẹo nhớ nhanh: Trước khi ấn Enter gửi câu hỏi cho AI, hãy tự hỏi: Mình đã cho AI biết bối cảnh chưa? Mình muốn nó đóng vai trò gì? Và mình muốn kết quả trả ra trông như thế nào?    
```
