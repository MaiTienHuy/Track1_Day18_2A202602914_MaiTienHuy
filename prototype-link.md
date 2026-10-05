# Prototype Link

Tài liệu này cung cấp liên kết truy cập và hướng dẫn chạy kiểm thử bộ ba micro-prototype A/B/C phục vụ nghiên cứu Case B: Hoàn thiện ghi chú sau bài giảng nhanh về kiến trúc RAG.

---

## 1. Danh sách file prototype chạy cục bộ

Cả ba prototype đều sử dụng chung tình huống học tập, ghi chú vội ban đầu và Slide 12:

| Option | File chạy trực tiếp | Cơ chế chính | Trạng thái kỹ thuật |
|---|---|---|---|
| **Option A** | [option-a.html](option-a.html) | Người học tự điền khung tư duy (Nhớ – Thiếu – Kiểm tra) | Độc lập, không lỗi runtime |
| **Option B** | [option-b.html](option-b.html) | Người học tự viết và gắn liên kết với Slide 12 | Độc lập, không lỗi runtime |
| **Option C** | [option-c.html](option-c.html) | Người học kiểm tra, sửa đổi hoặc xóa bỏ bản nháp AI mô phỏng | Độc lập, không lỗi runtime |

---

## 2. Hướng dẫn mở và kiểm thử trên máy tính

1. **Chuẩn bị file:** Tải toàn bộ thư mục bài nộp về máy tính và giải nén (nếu ở dạng file ZIP).
2. **Khởi chạy:** Nhấp đúp chuột hoặc chuột phải chọn mở file `option-a.html`, `option-b.html`, hoặc `option-c.html` bằng trình duyệt Google Chrome hoặc Microsoft Edge.
   - *Lưu ý:* Các file đều tự chứa đầy đủ mã nguồn HTML, CSS và JavaScript; không yêu cầu cài đặt môi trường, không cần node_modules hay kết nối internet.
3. **Trước mỗi lượt test:** Bấm nút *"Đặt lại cho tester mới"* (Reset) ở góc trên bên phải để đảm bảo dữ liệu của lượt dùng trước đã được làm sạch hoàn toàn.
4. **Quy trình kiểm thử:** Sử dụng đúng [Kịch bản 20 phút](test-plan.md) cho cả 3 option theo thứ tự xoay vòng đã phân công.

---

## 3. Thông tin Repository và Quyền truy cập

- **Tên Repository cá nhân chuẩn:** **`Track1_Day18_2A202602914_MaiTienHuy`**
- **Quyền truy cập:**
  - File mã nguồn và tài liệu markdown được mở công khai (Public) hoặc chia sẻ quyền đọc (Viewer) cho giảng viên và Teaching Assistant (TA).
  - Đã được kiểm tra mở độc lập bằng tài khoản ẩn danh (Incognito window), đảm bảo tất cả các file markdown và HTML đều hiển thị trơn tru, không bị lỗi phân quyền.
- **Link Design Sheet chung:** Xem trực tiếp tại [three-option-design-sheet.md](three-option-design-sheet.md) trong repository.

---

## 4. Các giới hạn kỹ thuật cần lưu ý

1. **Bộ nhớ phiên làm việc (In-memory state):** Prototype hoạt động trên bộ nhớ tạm của trình duyệt; việc tải lại trang (F5) hoặc đóng tab sẽ làm mới lại dữ liệu ghi chú ban đầu.
2. **Mô phỏng AI cố định:** Option C sử dụng một bản nháp mô phỏng cố định (fixed mock) được thiết kế có chủ đích cho tình huống RAG Slide 12, nhằm kiểm tra phản xạ đọc và thẩm định của người học; hệ thống không kết nối với API LLM bên ngoài.
3. **Ý nghĩa của thao tác xác nhận:** Việc tích checkbox *"Tôi đã đối chiếu..."* là hành động tự khai báo của người dùng; hệ thống prototype không tự động xác thực tính đúng sai của văn bản người dùng nhập vào.
