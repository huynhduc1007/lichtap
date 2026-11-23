# CLAUDE.md

Repo này là **Sổ Tập** (https://huynhduc1007.github.io/lichtap/): sổ tập, ăn uống, chạy bộ của Duc, gắn với Project "Gym". Nguyên tắc coaching, chấn thương, lịch tập nằm trong hướng dẫn của Project Gym. Khi sửa nội dung tập luyện hoặc dinh dưỡng trong app, theo đúng các nguyên tắc đó. Luôn trả lời bằng tiếng Việt.

## Làm việc với repo

- **Không commit thẳng vào `main`.** Mỗi thay đổi: tạo branch → commit → push → mở PR. Chỉ merge khi Duc nói rõ "merge".
- Toàn bộ app nằm trong một file `index.html` (HTML + CSS + JS, không build). GitHub Pages phục vụ từ `main`.
- **Giữ tương thích dữ liệu:** dữ liệu nằm trong `localStorage` khoá `pt-log-v1`. Không đổi tên khoá, không xoá trường cũ. Trường mới phải có giá trị mặc định trong `BLANK()`.
- Lịch race và các ngày đặc biệt nằm trong object `PLAN` (theo ngày), giai đoạn trong `PHASES`, bài tập trong `PROGRAM`. Mọi thay đổi chương trình hoặc dinh dưỡng phải thêm một dòng vào `CHANGELOG`, kèm lý do và nguồn (tác giả + năm).
- Trước khi mở PR: kiểm tra cú pháp JS và mở app ở khung 390 px, cả nền sáng lẫn tối, không có lỗi console.
- `sw.js` lưu đệm cho dùng offline. Khi đổi danh sách file cốt lõi thì tăng tên cache.
