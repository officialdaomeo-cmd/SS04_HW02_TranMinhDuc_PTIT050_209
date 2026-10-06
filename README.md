# Dự án quản lý nhánh

Đây là nội dung đã được giải quyết xung đột bằng cách kết hợp cả hai nhánh:
- Nhánh main: Đây là nội dung được thay đổi ở nhánh main để tạo conflict.
- Nhánh feature-update: Đây là nội dung được thay đổi ở nhánh feature-update.

## Báo cáo giải quyết xung đột
1. Khởi tạo repository, tạo file README.md và commit ban đầu trên nhánh `main`.
2. Tạo nhánh `feature-update` từ `main`, thay đổi nội dung file README.md, và commit.
3. Chuyển lại về nhánh `main`, thay đổi cùng dòng trên file README.md, và commit để tạo xung đột.
4. Thực hiện lệnh `git merge feature-update` trên nhánh `main` dẫn đến thông báo Merge Conflict.
5. Mở file README.md, tìm các đoạn có ký hiệu đánh dấu xung đột (`<<<<<<< HEAD`, `=======`, `>>>>>>> feature-update`).
6. Xóa các ký hiệu này và chỉnh sửa lại nội dung file cho phù hợp.
7. Lưu file, chạy lệnh `git add README.md` và `git commit` để hoàn thành việc gộp nhánh (Merge Commit).
8. Dùng lệnh `git log --graph --oneline` để kiểm tra lịch sử commit.
