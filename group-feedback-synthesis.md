# Group Feedback Synthesis — Nhóm DBH · Case B

Ba phiên, mỗi tester ngoài nhóm thử cả A/B/C, thứ tự xoay vòng.

| Nội dung | Feedback 1 — Đạt (tester: Ninh Quang Minh, A→B→C) | Feedback 2 — Biển (tester: Trần Phạm Thái Vũ, B→C→A) | Feedback 3 — Huy (tester: Đinh Trường An, C→A→B) | Pattern hoặc khác biệt |
|---|---|---|---|---|
| First action | A, B: bấm lưu ngay khi ô đã có sẵn chữ; C: bấm tạo bản nháp | B: bấm vào ô ghi chú; C: bấm tạo bản nháp nhanh; A: bấm vào ô "Điều tôi nhớ" | C: đọc nhãn mô phỏng rồi đọc lướt bản nháp; A: đọc các ô rồi điền "RAG = lấy doc nhét vào prompt"; B: bấm gắn slide trước, rồi mới viết ghi chú | Ở C, cả ba đều tạo bản nháp ngay; ở A/B, nội dung điền sẵn khiến có người lưu luôn |
| Breakdown chính | B: bước "gắn ghi chú vào Slide 12" không hiển nhiên dù nguồn hiện sẵn; C: đổi ghi chú đầu vào nhưng bản nháp không đổi, xóa trắng bản nháp vẫn lưu được | A: dừng lâu nhất ở ô việc cần kiểm tra; B: slide không giải thích hết điều muốn biết | C: dừng ở cảnh báo giới hạn lời giảng, hỏi ví dụ vector search có phải AI tự thêm không; A: bế tắc ở ô "Điều còn thiếu" vì không nhớ giảng viên nói thêm gì; B: phân vân gắn slide thì mai mở ra thấy cả bài giảng hay chỉ slide, lo nhiều slide sẽ bị loạn | A khó khi người học không còn nhớ lời giảng; B giữ nguồn nhưng không giúp hiểu nội dung |
| Cách lấy lại control | Dùng được các đường sửa, bỏ, gắn lại; C buộc tick xác nhận trước khi lưu | Không sửa nội dung ở B và C; tick xác nhận rồi lưu ở C | C: bỏ bản nháp, tạo lại, tự sửa một dòng (thêm lưu ý về reranking), tick rồi lưu; A: sửa lại ô; B: bỏ gắn rồi gắn lại trước khi lưu | Ai cũng tìm được đường sửa/bỏ mà không cần trợ giúp; nhưng ô tick ở C không đảm bảo có kiểm tra thật |
| Option được chọn | **B** | **C** | **C** | 2 chọn C, 1 chọn B; cả ba lý do đều xoay quanh **nguồn và khả năng kiểm chứng** |
| Trade-off | Chọn B vì thấy rõ liên hệ giữa ghi chú và Slide 12; chưa tin C vì bản nháp không phản ứng với ghi chú và bản lưu mất nhãn nguồn | Chọn C vì "nhanh nhất mà vẫn có bước kiểm tra", nhưng vẫn muốn tự kiểm tra đúng sai | Chọn C vì không phải viết nhiều sau buổi học mệt, chỉ cần đóng vai người kiểm duyệt, và vì sửa, xóa được; vẫn mất 1–2 phút đọc lại vì chưa dám tin; muốn thấy nổi bật chỗ khác nhau giữa slide và bản nháp | Người học sẵn sàng giao AI viết nháp, nhưng chỉ khi thấy được nội dung đến từ đâu |

## Pattern chính
1. **Nguồn là điều cả ba tester cần**, dù chọn B hay C: Minh chọn B vì rõ nguồn; Vũ đọc nguồn trước khi lưu; An đối chiếu bản nháp với slide, nghi ngờ ý AI tự thêm và muốn thấy rõ chỗ khác nhau.
2. **Bước xác nhận ở C chưa làm đúng việc của nó**: Vũ tick mà không sửa gì; An nói khi vội người ta vẫn tick mà không đọc; Minh lưu được bản nháp rỗng và bản lưu cuối mất nhãn nguồn.
3. **A tốn công nhất** và khó khi người học không nhớ lời giảng (cả ba đều dừng ở các ô "còn thiếu" hoặc "cần kiểm tra").
4. **B giữ nguồn nhưng không giúp hiểu nội dung**, và thao tác gắn nguồn chưa hiển nhiên.

## Một Next Change nhóm chốt
**Giữ cơ chế chính của C (AI viết nháp, người học duyệt và quyết định lưu) và thay ô tick xác nhận bằng nguồn gắn theo từng câu kiểu B:** mỗi câu nháp chỉ rõ đến từ slide hay do AI tự diễn giải, người học giữ, sửa hoặc bỏ từng câu, không lưu được bản rỗng, và nhãn nguồn được giữ trên ghi chú đã lưu.

**Evidence dẫn tới quyết định:** cả ba tester đều dựa vào nguồn để quyết định tin hay không (pattern 1); ô tick bị bỏ qua hoặc không ngăn được bản lưu sai (pattern 2); hai trên ba tester chọn C vì đỡ công viết, còn tester chọn B làm vậy vì nguồn rõ hơn.

## Still Unproven sau ba feedback
- Người học có thật sự đọc nguồn từng câu khi tự học lúc vội hoặc buổi tối, không có người quan sát.
- Ghi chú tạo ra có giúp làm bài tập ngày hôm sau tốt hơn không (chưa test việc dùng lại ghi chú).
- Kết quả với người mới học: cả ba tester đều đã học RAG, có nền tảng để soi lỗi AI.
- Cách hiển thị nguồn khi một buổi học có nhiều slide (lo ngại của An).
- Ba feedback không đủ để kết luận C tốt hơn B hay A.

**Kết luận:** Với Hypothesis Problem này, chúng tôi đã thử ba cách giải. Tester đã chọn C hai lần và B một lần, nhưng cả ba đều dựa vào nguồn để quyết định có tin nội dung hay không, và ô tick xác nhận ở C không đảm bảo việc kiểm tra thật; vì vậy iteration tiếp theo chúng tôi sẽ kết hợp bản nháp của C với nguồn theo từng câu của B rồi test lại với người học mới hơn. Kết quả này chưa chứng minh solution đã được validated.

**Giới hạn dữ liệu:** Feedback 1 thiếu ngày test và câu trả lời bối cảnh của tester. Feedback 3 dùng một số tên nút và nội dung bản nháp khác bản prototype chung, có thể do phiên đó dùng biến thể của prototype; tổng hợp giữ nguyên ghi chép như người facilitate báo cáo.
