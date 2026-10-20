# Little Moon — website mẫu cho GitHub Pages

## Các trang
- `index.html`: trang chủ với ảnh minh họa trong `assets/hero.png`
- `posts.html`: danh sách bài viết
- `qa.html`: gửi câu hỏi ẩn danh và xem phản hồi
- `about.html`: thông tin cá nhân
- `admin.html`: giao diện demo để viết bài và trả lời Q&A
- `style.css`, `app.js`: giao diện và hành vi dùng chung

## Chạy thử
Mở `index.html` bằng trình duyệt. Có thể dùng VS Code + Live Server để chạy tiện hơn.

## Đưa lên GitHub Pages
1. Tạo repository trên GitHub.
2. Tải các file và thư mục trong dự án lên repository (giữ nguyên cấu trúc).
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**, chọn nhánh `main` và thư mục `/ (root)`, bấm Save.
5. Đợi GitHub Pages triển khai xong rồi mở URL được cung cấp.

## Giới hạn rất quan trọng
Bản này là front-end demo. Bài viết/câu hỏi/câu trả lời được lưu trong `localStorage`, tức chỉ có trên trình duyệt và thiết bị hiện tại. Dữ liệu không đồng bộ giữa khách truy cập, không phải cơ sở dữ liệu chung.
`admin.html` chưa có xác thực và không an toàn để quản trị nội dung trên website công khai. Không đưa mật khẩu bí mật vào HTML/JavaScript. Để dùng thật, cần tích hợp backend/cơ sở dữ liệu (ví dụ Supabase hoặc Firebase) và xác thực quản trị, đồng thời cấu hình quyền truy cập để khách chỉ gửi câu hỏi còn chỉ quản trị viên được trả lời/xóa.
