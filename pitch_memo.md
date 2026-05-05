# PITCH MEMO — MindMesh

1. THE PROBLEM 

   Sinh viên và nghiên cứu sinh phải đọc hàng chục paper cho mỗi topic, mất nhiều ngày chỉ để xác định bài nào đáng đọc sâu. Quá trình literature review lặp lại theo từng deadline, tiêu tốn nhiều thời gian nhưng phần lớn effort lại dành cho việc lọc và skim thay vì hiểu sâu.

2. THE INSIGHT

   - Người dùng không cần AI “đọc thay toàn bộ paper” — họ cần một cách đáng tin để nhanh chóng quyết định paper nào đáng đọc và paper nào có thể bỏ qua. 
   - Vốn không nên thay thế được việc đọc toàn bộ, nhưng thật sự có quá nhiều hướng một chủ đề có thể xoay quanh, và mỗi paper xuất bản ra hàng ngày không phải lúc nào có nội dung đáng chú ý hoặc chất lượng, việc phải đọc khiến cho đối tượng hướng tới - sinh viên và nghiên cứu sinh dễ nản, đặc biệt dưới tình trạng có deadline.


3. THE SOLUTION

   - Sản phẩm cung cấp một hệ thống tìm kiếm và tóm tắt paper theo truy vấn, trả về danh sách các bài liên quan kèm tóm tắt “đủ để ra quyết định”, trích dẫn rõ ràng và metadata để kiểm chứng nhanh.
   - Khác với ChatGPT hoặc các công cụ tóm tắt đơn lẻ, hệ thống tập trung vào **decision support** (rank + summary + synthesis + source-grounded), giúp người dùng chọn đúng paper thay vì chỉ đọc nhanh hơn.
   - AI được sử dụng để tổng hợp thông tin có kiểm soát (grounded summaries and synthesis), trong khi retrieval và ranking kết hợp heuristic để giảm hallucination và tăng độ tin cậy.

4. WHY NOW

   Sự phổ biến của arXiv và các kho học thuật khiến số lượng paper tăng nhanh, vượt quá khả năng xử lý thủ công của người học. Đồng thời, LLM hiện tại đã đủ tốt để tạo summary có nguồn đáng tin, nhưng chưa được đóng gói thành workflow phù hợp với quá trình literature review thực tế.

5. TRACTION / PROOF (số cụ thể)

   - Số người dùng / pilot: 50-80 người dùng thử ban đầu.
   - Aha moment metric: ngưỡng 40-50% user đạt trong session đầu có thể chọn được ít nhất 1-2 paper ưng ý, ~30% quay lại sử dụng trong vòng 7 ngày khi tiếp tục làm assignment / research.
   - LTV/CAC, payback: 2.92x, 4.3 tháng. 

6. THE ASK (1-2 câu)

   Em cần 100,000,000VND–200,000,000VND pre-seed funding để hoàn thiện MVP, tối ưu cost pipeline và đạt ~500–1,000 người dùng hoạt động trong 12 tháng tới. Ngoài ra, cần hỗ trợ từ mentor và các đối tác trong lĩnh vực học thuật để tiếp cận user thật và validate hành vi sử dụng ở quy mô lớn hơn.