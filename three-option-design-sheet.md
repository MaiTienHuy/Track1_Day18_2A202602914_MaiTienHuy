# Three-Option Design Sheet — Nhóm DBH · Case B (AI Notes)

**Thành viên:** Phạm Quốc Đạt (2A202602384) · Nguyễn Văn Biển (2A202602416) · Mai Tiến Huy (2A202602914)
**Phụ trách option:** A: Phạm Quốc Đạt · B: Nguyễn Văn Biển · C: Mai Tiến Huy

## 1. Evidence Snapshot (từ Day 17)

| Practice Note | User đã thực sự làm/nói | Điều nhóm diễn giải |
|---|---|---|
| Đạt | Trong buổi học về RAG, chỉ kịp ghi đề mục/từ khóa vì giảng viên nói nhanh; về nhà có thể quên hoặc nhớ sai; tìm hiểu lại hoặc hỏi AI | Ghi chú thiếu lời giảng khiến người học không chắc mình hiểu đúng |
| Biển | Ghi chú slide và bài giảng trên VLearn; ôn ở nhà bằng AI rút ý chính từ slide kết hợp video rồi tự tổng hợp; chỉ đọc lại khi cần hoặc có bài kiểm tra; nói ghi tay mất thời gian nhưng "không hoàn toàn là mất thời gian" | Đã có workaround bằng AI; việc tự ghi có giá trị ghi nhớ |
| Huy | Có tóm tắt về việc dùng Ctrl+F và quên mở ghi chú, nhưng không có ghi chép gốc | Không dùng làm evidence |

- **Lặp lại:** cả hai note có evidence đều dùng AI sau buổi học.
- **Mâu thuẫn:** note của Biển không gặp chuyện ghi không kịp, và coi việc tự ghi là có ích.
- **Vẫn là suy đoán:** ghi thiếu có xảy ra thường xuyên và gây hậu quả thật không.

**Hypothesis Problem:**
> Khi học một buổi có nhiều kiến thức/từ khóa trình bày nhanh, learner gặp khó khăn trong việc ghi lại đủ phần giải thích cho khái niệm chưa hiểu vì không ghi kịp lời giảng, dẫn đến ghi chú chỉ còn từ khóa, khi xem lại không chắc mình hiểu đúng và phải tìm hiểu lại.

- **Evidence ban đầu:** note của Đạt.
- **Chưa chứng minh:** tần suất và hậu quả thật; người học có muốn giao việc ghi chú cho AI không. Practice interview Day 17 không phải validation.

## 2. Ba Solution Options

**Solution Parking Lot (Day 17):** đánh dấu nhanh chỗ chưa hiểu · template ghi chú · liên kết ghi chú với slide · AI tóm tắt có cấu trúc · AI gợi ý ngữ cảnh. Pool đã có hướng không dùng AI và nhiều cơ chế nên không bổ sung. Nguyên lý adapt từ Day 16 (Cursor): **mức tự chủ của AI**, từ người dùng tự làm đến AI làm rồi người dùng duyệt.

**Giữ nguyên cho A/B/C**

| Thành phần | Quyết định chung |
|---|---|
| Target user | Học viên học online trên VLearn |
| Situation | Buổi học nhanh, chỉ kịp ghi "RAG — lấy tài liệu trước khi AI trả lời?" |
| Task | Chuẩn bị một ghi chú để ngày mai xem lại khi làm bài tập |
| Desired outcome | Ghi chú đủ để hiểu lại ý và biết cần kiểm tra gì thêm |
| Content fixture | Slide 12 mẫu: "Truy xuất tài liệu liên quan → đưa vào ngữ cảnh → AI tạo câu trả lời"; slide không ghi nguyên văn lời giảng |

**Được phép khác**

| Thành phần | A — Ghi chú theo khung | B — Ghi chú gắn với nguồn | C — Bản nháp AI có kiểm chứng |
|---|---|---|---|
| Mechanism | Người học tự điền: từ khóa, điều nhớ, phần còn thiếu, việc cần kiểm tra | Người học gắn ghi chú vào Slide 12 để mở lại cùng ngữ cảnh | AI tạo bản nháp từ ghi chú vội và slide; người học sửa, xác nhận hoặc bỏ |
| User làm gì | Tự viết toàn bộ | Đối chiếu, gắn nguồn, ghi điều cần kiểm tra | Đọc, sửa, tick xác nhận rồi lưu |
| AI/hệ thống làm gì | Không làm gì | Hệ thống lưu liên kết, không suy luận | AI viết bản nháp (canned output) |
| Trigger | Người học mở khung | Người học bấm gắn nguồn | Người học bấm tạo bản nháp |
| Trade-off chính | Tự nghĩ giúp nhớ, nhưng tốn công viết | Rõ nguồn, nhưng không giúp diễn giải nội dung | Nhanh, nhưng phải kiểm tra vì AI có thể thêm ý ngoài slide |

**Distance check**
- A khác B vì: ở A người học tự diễn giải trong khung; ở B người học không thêm diễn giải mà gắn ghi chú với nguồn.
- B khác C vì: ở B nội dung là của người học, chỉ thêm nguồn; ở C AI viết nội dung, người học duyệt.
- A khác C vì: người học tạo hoàn toàn so với AI tạo, người học duyệt.

**Giới hạn đã biết:** A và B đều không có AI suy luận; B chỉ thể hiện vai trò của hệ thống (liên kết nguồn).

## 3. Human–AI Decision Table

**Critical interaction:** biến ghi chú vội về RAG thành ghi chú dùng được cho buổi ôn hôm sau.

| Human–AI decision | A | B | C |
|---|---|---|---|
| User làm gì? AI làm gì? | User viết, lưu; AI không làm gì | User đối chiếu và gắn nguồn; hệ thống lưu liên kết | User sửa, xác nhận, quyết định lưu; AI viết nháp |
| Act / Ask / Don't Act? Vì sao? | **Don't Act**: giữ giá trị tự ghi | **Don't Act**: hệ thống chỉ liên kết theo thao tác của người học | **Act, chờ xác nhận**: tiết kiệm công viết; không lưu khi chưa xác nhận |
| User hiểu capability/limit bằng gì? | Dòng "Tự điền theo cách bạn hiểu" | Mô tả gắn ghi chú với slide; dòng "Nguồn slide không ghi nguyên văn lời giảng" | Dòng "AI không biết chính xác giảng viên nói gì ngoài slide"; nhãn "Bản nháp AI · cần bạn kiểm tra" |
| Evidence/uncertainty thể hiện thế nào? | Người học tự ghi phần còn thiếu, chưa chắc | Nguồn Slide 12 hiển thị cùng ghi chú đã lưu | Khung "Phần có nguồn · Slide 12"; câu "phần giải thích nói thêm chưa được xác minh" |
| Kiểm soát và recovery | Sửa sau khi lưu | Bỏ gắn, sửa ghi chú, xem lại nguồn sau khi lưu | Sửa trực tiếp, bỏ bản nháp, sửa hoặc bỏ bản đã lưu |

**Feedback and data check:** chỉ dùng ghi chú vội và Slide 12; dữ liệu chỉ giữ trong phiên trình duyệt; người học bỏ hoặc sửa được bất cứ lúc nào.

## 4. Prototype

Mỗi option: bối cảnh chung → tương tác chính → ghi chú đã lưu. Bản nháp của C là canned output, không gọi AI thật. Ba file HTML trong `prototype/` là đúng phiên bản đã dùng để test.
