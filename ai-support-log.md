# AI Support Log

**Học viên thực hiện:** Mai Tiến Huy (MHV: 2A202602914)  
**Nhóm:** Nhóm 6 (Case B — Hoàn thiện ghi chú sau một buổi học diễn ra nhanh)  
**Vai trò cá nhân:** Phụ trách thiết kế tương tác Option C (Bản nháp AI có kiểm chứng) và trực tiếp điều phối phiên test số 3.

---

## AI đã hỗ trợ gì?

| Công việc trong quá trình làm Lab | Nội dung AI hỗ trợ | Giới hạn & Cách tôi sử dụng kết quả |
|---|---|---|
| **Rà soát code và logic của 3 prototype A/B/C** | Phân tích mã nguồn HTML/JS của 3 option; chỉ ra rằng Option C sử dụng bản nháp cố định (hard-coded mock), dữ liệu mất khi tải lại trang, và phát hiện trạng thái nút bấm chưa tối ưu khi người dùng reset. | Tôi dùng góp ý này để hiểu rõ các ràng buộc kỹ thuật của prototype; ghi rõ trong tài liệu giới thiệu rằng đây là prototype mô phỏng, không lừa dối tester rằng hệ thống đang gọi LLM thật. |
| **Bóc tách tương tác Human–AI** | Giúp định hình 4 thành tố kiểm soát của người dùng: Expectation (Kỳ vọng), Agency (Quyền năng), Evidence/Uncertainty (Bằng chứng/Sự không chắc chắn), và Recovery (Đường khôi phục). | Giúp tôi thiết kế nút "Bỏ bản nháp" (Discard) và checkbox xác nhận ở Option C; không để AI tự động lưu ghi chú khi người học chưa can thiệp. |
| **Thiết kế kịch bản kiểm thử 20 phút** | Đề xuất khung thời gian chuẩn (0–2' làm quen, 2–14' dùng A/B/C, 14–18' so sánh trade-off, 18–20' ghi chú); cung cấp các câu hỏi mở và câu nhắc trung tính để facilitator không dẫn dụ tester. | Tôi sử dụng nguyên văn bộ câu nhắc trung tính này trong suốt 20 phút chạy test với Tester 3 để đảm bảo tính khách quan của quan sát. |
| **Cấu trúc hồ sơ nộp bài theo 5 Gate** | Hướng dẫn định dạng markdown cho `README.md`, `prototype-feedback-note.md`, `group-feedback-synthesis.md` bám sát các tiêu chí khắt khe của rubric. | Dùng làm khung sườn lưu trữ dữ liệu; toàn bộ nội dung quan sát và phân tích hành vi do nhóm tự điền dựa trên bằng chứng kiểm thử thực tế. |

---

## AI đã sai hoặc còn hời hợt ở đâu?

1. **Sai lệch nghiêm trọng về phân công test:**
   - *Chi tiết:* Khi tôi thông báo mình phụ trách Option C, AI ban đầu gợi ý: *"Vậy bạn chỉ cần tập trung cho tester dùng thử thật kỹ Option C để lấy feedback sâu"*.
   - *Nhận diện & Sửa lỗi:* Đây là tư vấn sai hoàn toàn so với yêu cầu bắt buộc của Chặng 6. Đề bài quy định rõ: Dù phụ trách option nào, mỗi thành viên đều phải cho tester của mình thử **cả ba option A, B và C**. Tôi đã ngay lập tức bác bỏ gợi ý này của AI và tuân thủ quy trình xoay vòng thứ tự (C → A → B).
2. **Thiên kiến "thần thánh hóa AI" và tạo dữ liệu khen ngợi một chiều (Violation of Gate 5):**
   - *Chi tiết:* Trong một số gợi ý phản hồi mẫu ban đầu, AI có xu hướng đưa ra các phát biểu hư cấu kiểu *"Tester rất thích C vì AI viết văn phong mượt mà, giúp tiết kiệm 90% thời gian"*.
   - *Nhận diện & Sửa lỗi:* Đây là biểu hiện hời hợt, vi phạm tiêu chí "Learning, not praise" của Gate 5. Tôi đã chặn đứng xu hướng này và yêu cầu tập trung vào **các điểm nghẽn hành vi (breakdowns)**, sự nghi ngờ của tester, và việc Tester 1 (Khoa) kiên quyết từ chối C để chọn B vì sợ AI bịa đặt.
3. **Mô tả sai bản chất của Prototype C:**
   - *Chi tiết:* AI nhiều lần dùng cụm từ *"AI sẽ phân tích câu ghi chú của bạn để sinh ra văn bản"*.
   - *Nhận diện & Sửa lỗi:* Tôi đã nhắc nhở và chỉnh sửa lại: Prototype C trong bài lab này không gọi API backend, mà chỉ nạp một đoạn nháp cố định được soạn sẵn để kiểm tra phản xạ đọc - sửa - duyệt của người học. Việc nói quá về AI sẽ làm sai lệch bản chất của phép thử usability.
4. **Vội vã tuyên bố giải pháp đã được xác thực (Validated):**
   - *Chi tiết:* AI từng đề xuất kết luận rằng *"Nhóm đã tìm ra giải pháp tối ưu cho bài toán ghi chú sau giờ học"*.
   - *Nhận diện & Sửa lỗi:* Tôi đã gạch bỏ kết luận này. Với 3 người dùng trong 20 phút tại phòng lab, giải pháp hoàn toàn **chưa thể coi là validated**. Tôi đã tự viết lại mục *Still Unproven* với 4 điều chưa biết về hiệu quả học tập dài hạn.

---

## Tôi đã tự kiểm tra, sửa hoặc bác bỏ gì?

- **Kiểm tra giao diện và mã nguồn prototype:**
  - Tự tay mở cả 3 file `option-a.html`, `option-b.html`, `option-c.html` trên trình duyệt Microsoft Edge và Chrome.
  - Thử nghiệm các tình huống biên (edge cases): Thử bấm Lưu khi textarea rỗng; thử bấm "Bỏ bản nháp" rồi tạo lại; thử bấm nút "Đặt lại cho tester mới" để xác nhận trạng thái reset hoạt động trơn tru trước khi bắt đầu phiên test chính thức.
- **Tự điều phối và ghi chép phiên test thực tế:**
  - Trực tiếp mời bạn Vũ Hoàng Long (học viên ngoài nhóm) tham gia phiên test 20 phút.
  - Tuyệt đối giữ im lặng trong 3 phút đầu của mỗi option, không can thiệp, không chỉ tay vào nút bấm, chỉ quan sát hướng mắt và thao tác chuột của tester.
  - Ghi lại trung thực từng câu nói ngập ngừng, thắc mắc về cụm từ "Retriever" và hành động bấm nút "Bỏ bản nháp" của Long.
- **Đóng góp quyết định thiết kế của nhóm:**
  - Tại buổi tổng hợp của nhóm, tôi là người đề xuất **không loại bỏ Option B**, mà kết hợp tính năng neo nguồn (Slide anchoring) của B vào trong Option C để giải quyết vấn đề hoài nghi của người học.
  - Đề xuất thay thế checkbox xác nhận tĩnh bằng cơ chế so sánh trực quan (Visual Diff) để chống lại thói quen tick bừa của người dùng.
- **Bài học cá nhân rút ra:**
  - AI là một trợ thủ đắc lực trong việc cấu trúc hóa tài liệu và tư duy phản biện ngược, nhưng nó có "điểm mù" rất lớn là luôn có xu hướng khen ngợi các giải pháp ứng dụng AI.
  - Nếu người làm sản phẩm không giữ được cái đầu lạnh và không dựa vào hành vi thực tế của người dùng, sản phẩm sẽ rất dễ rơi vào bẫy "giải pháp tìm kiếm vấn đề" (a solution looking for a problem).

---

