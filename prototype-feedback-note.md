# Prototype Feedback Note — phiên cá nhân

**Người thực hiện:** Mai Tiến Huy (Option c)  

---

## Thông tin

- **Người thực hiện:** Mai Tiến Huy (MHV: 2A202602914)
- **Tester:** Đinh Trường An - 2A202602393 (học viên lớp AI Product K12, vừa hoàn thành bài học lý thuyết và đang chuẩn bị làm bài tập lập trình về pipeline RAG - Retrieval-Augmented Generation).
  - *Relevant context:* Thường sử dụng các công cụ AI như ChatGPT để tóm tắt bài giảng nhưng hay phàn nàn rằng AI sinh nội dung quá dài dòng, không bám sát yêu cầu nộp bài của giảng viên và dễ gây "ảo tưởng là mình đã hiểu". Khi nghe giảng nhanh, An hay gõ vội câu hỏi vào app ghi chú rồi sau đó quên mở lại.
- **Thứ tự thực hiện:** **C → A → B**

---

## OBSERVED — hành vi và lời nói thực tế

| Observation | Option C (thử đầu tiên) | Option A (thử thứ hai) | Option B (thử thứ ba) |
|---|---|---|---|
| **First action** | Đọc qua nhãn "AI mô phỏng cố định", sau đó đọc lướt 5 dòng đầu của khung bản nháp. | Đọc 3 ô: "Điều tôi nhớ", "Điều còn thiếu", "Việc cần kiểm tra". Thao tác vào các ô: *"RAG = lấy doc nhét vào prompt"*. | Bấm nút *"Gắn Slide 12 vào ghi chú"*. Nhìn sang khung preview slide bên cạnh rồi mới bấm vào ô text ghi chú. |
| **Chỗ dừng** | Dừng lại ở cảnh báo: *"Slide không ghi nguyên văn lời giảng; AI không thể phục hồi những gì thầy nói ngoài slide"*. Hỏi lại: *" cái ví dụ vector search trong này là AI tự bịa thêm à?"*. | Dừng lại ở ô *"Điều còn thiếu"*. Nói: *"Lúc giảng nhanh quá tôi còn chẳng biết thầy nói thêm cái gì thì làm sao biết mình thiếu cái gì mà điền"*. | Khi đọc tiêu đề slide: *"Truy xuất tài liệu liên quan → đưa vào ngữ cảnh..."*. Phân vân liệu bấm "Gắn slide" thì mai mở ra có thấy nguyên bài giảng hay chỉ thấy mỗi cái ảnh slide này. |
| **Evidence được đọc / bỏ qua / chưa rõ** | **Đã đọc:** Nhìn sang Slide 12 bên trái để so sánh từ *"Truy xuất"* với từ *"Retriever"* trong bản nháp AI. Nói: *"Slide ghi tiếng Việt, AI viết tiếng Anh kèm theo"*. | Nhìn qua Slide 12 để tìm ý điền vào ô "Điều còn thiếu", nhưng không chép nguyên văn mà cố nhớ lại lời giảng. | **Đã đọc kỹ:** Đọc kỹ từng bước mũi tên trên Slide 12 để viết vào ô ghi chú cá nhân; dùng chính xác cụm *"đưa vào ngữ cảnh"*. |
| **Cách tester sửa** | Bấm nút *"Bỏ bản nháp đề xuất"*. Bản nháp biến mất, quay về ghi chú ban đầu. Nói: *"nghĩ là phải dừng nhưng lại xóa được"*. Sau đó bấm tạo lại bản nháp, sửa trực tiếp dòng số 2 trong textarea (thêm lưu ý về reranking), tick checkbox xác nhận và bấm Lưu. | Viết sai ở ô 1, bấm Ctrl+Z để xóa và viết lại. Cảm thấy ô 3 (Việc cần kiểm tra) khó nghĩ nên chỉ ghi: *"Hỏi lại trợ giảng về vector db"*. | viết thử vào ghi chú sau đó bấm *"Bỏ gắn slide"* để xem giao diện, rồi bấm *"Gắn lại"* trước khi bấm Lưu. |
| **Tự hoàn thành hay cần trợ giúp** | Tự hoàn thành, Tôi chỉ đọc hướng dẫn và nhiệm vụ chung theo kịch bản. | Tự hoàn thành; facilitator giữ im lặng hoàn toàn. | Tự hoàn thành; tester tự giải thích thao tác khi bấm gắn slide. |
| **Phần vẫn chưa chắc** | *"Chưa chắc mai đi học thầy có bắt dùng đúng thuật ngữ tiếng Anh như AI viết không, hay phải theo slide tiếng Việt"*. | *"Ghi thế này mai đọc lại chưa chắc đã hiểu, cảm giác tự ghi thì vẫn bị hổng kiến thức"*. | *"Nếu bài có 40 slide mà cái nào cũng gắn thế này thì lúc mở ghi chú ra có bị loạn không?"*. |
| **Hành vi trước và sau thử sửa** | Trước: Đã tự sửa textarea 1 lần trước khi lưu. Sau khi được yêu cầu thử sửa: Bấm ngay nút *"Quay lại sửa ghi chú"*, thêm tag #quan-trong vào cuối văn bản và lưu lại. | Bấm nút sửa, bổ sung thêm 1 gạch đầu dòng ở ô "Việc cần kiểm tra". | Bấm sửa nội dung text, không đụng vào nút gắn slide. |
| **Evidence** | Nhóm từng lo ngại tester sẽ bị "lười" và bấm Lưu ngay mà không đọc; thực tế Tester đọc rất kỹ câu cảnh báo và hoài nghi nội dung AI viết, chủ động bấm "Bỏ bản nháp" để kiểm tra trước khi chấp nhận sửa. | Nhóm kỳ vọng khung 3 phần sẽ giúp người học tư duy sâu; thực tế tester bị bế tắc và ức chế ở ô "Điều còn thiếu" vì không đủ dữ liệu nhớ lại. | Nhóm nghĩ gắn slide là trực quan nhất; nhưng tester lại nhận xét rằng gắn slide chỉ giải quyết phần ngọn, lúc mở ra vẫn phải tự đọc lại slide từ đầu nếu không có phần tổng hợp ý nghĩa. |

---

## Compare — sau cả ba option

| Nội dung | Note thực tế từ phát biểu của Tester 3 |
|---|---|
| **Option được chọn** | **Option C (Bản nháp AI có kiểm chứng)** |
| **Lý do lựa chọn** | Sau một buổi học mệt mỏi mà phải viết thêm 3 ô như option A thì rất dài. Option C cho thấy một điểm bắt đầu rõ ràng, chỉ việc đóng vai người kiểm duyệt xem nó viết đúng hay sai. Nhưng chọn C chỉ vì cho phép sửa và xóa. |
| **Muốn tự làm gì, giao cho AI gì?** | - **Giao cho AI:** Tóm tắt các bước chính từ slide và ghi chú vội thành một bản nháp có cấu trúc rõ ràng để bắt đầu. Tự làm: Đọc lại đối chiếu với slide, sửa hoặc xóa những từ ngữ AI viết thừa/thầy không dạy, thêm các lưu ý cá nhân để mai làm bài tập. |
| **Điều chưa thoải mái** | - Điểm chưa thoải mái: Checkbox *"Tôi đã đối chiếu..."*  nếu đang vội thì người ta vẫn bấm lưu mà không đọc. Nên có cách nào làm nổi bật điểm khác biệt giữa slide và bản nháp để dễ nhìn hơn.  Vẫn phải tốn 1–2 phút ngồi đọc lại xem AI viết đúng không chứ không dám tin ngay. |

---

## INTERPRETED — cách tôi hiểu observation

Người học có tâm lý cảnh giác lành mạnh và cần đường rút lui an toàn khi cộng tác với AI (Option C), trong khi việc bắt buộc nhớ lại thuần túy mà thiếu tài liệu gợi nhắc (Option A) rất dễ gây quá tải nhận thức. Dù vậy, phản xạ soi lỗi AI này một phần có thể đến từ việc tester (An) đã có sẵn nền tảng kiến thức từ trước chứ chưa chắc phản ánh đúng hành vi của người mới bắt đầu.

---

## DECIDED — NEXT CHANGE (Đề xuất cá nhân sau phiên)

Tôi đề xuất giữ cơ chế đồng kiểm soát của Option C nhưng tích hợp thêm neo nguồn từ Option B: khi bấm vào câu nháp AI thì slide bài giảng tương ứng sẽ tự động sáng đèn (highlight), đồng thời chỉ mở nút Lưu khi người học đã thực sự click đối chiếu hoặc chỉnh sửa nhằm triệt tiêu thói quen tick quán tính. Thay đổi này được giữ lại để thảo luận tại buổi Group Synthesis chứ không sửa prototype ngay nhằm bảo đảm tính nhất quán dữ liệu cho nhóm.

---

## STILL UNPROVEN (Điều chưa thể kết luận từ phiên cá nhân)

Phiên test 20 phút có người quan sát vẫn chưa thể chứng minh hiệu quả ghi chú khi áp dụng vào bài tập thực tế ngày hôm sau. Đồng thời, nguy cơ người học bấm Lưu mù quáng khi tự học lúc đêm muộn (automation fatigue / hiệu ứng Hawthorne) và mức độ hiệu quả đối với học viên hoàn toàn mất gốc vẫn là những câu hỏi còn bỏ ngỏ cần kiểm chứng thêm.

---
