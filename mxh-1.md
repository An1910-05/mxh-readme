
### 2. Mục tiêu dự án

* Xây dựng bản demo/prototype cho các chức năng cốt lõi của mạng xã hội.
* Tách riêng **giao diện** và **API** để dễ mở rộng, bảo trì và phát triển thêm sau này. 

### 3. Các chức năng chính

Bạn nên gom thành 1 slide hoặc 2 slide:

* **Xác thực**: đăng ký, đăng nhập, JWT, Google login, quên mật khẩu.
* **Hồ sơ cá nhân**: avatar, ảnh bìa, bio, URL cá nhân.
* **Bài viết và tương tác**: tạo/sửa/xóa bài, like, comment, reaction.
* **Thông báo**: thông báo bình luận, nhắc tên, badge chưa đọc.
* **Quan hệ người dùng**: follow, kết bạn, lời mời kết bạn.
* **Chat realtime**: nhắn tin qua REST + WebSocket.
* **Tìm kiếm, stories, upload media, link preview**. 

### 4. Cập nhật nổi bật gần đây

Chỉ nên chọn vài điểm mạnh, không cần nói hết:

* **Nạp tiền qua VNPay**.
* **Trang Cài đặt tài khoản**.
* **Đăng nhập Google**.
* **Sidebar trái + mục Trò chơi**.
* **Reaction chi tiết và xem ai đã thả reaction**. 

### 5. Kiến trúc hệ thống

Nên nói ngắn gọn:

* Frontend gọi **REST/GraphQL** tới backend.
* Chat realtime dùng **WebSocket**.
* Dữ liệu lưu ở **MySQL**.
* Hệ thống đóng gói bằng **Docker Compose** nên dễ triển khai local hoặc VPS. 

### 6. Công nghệ sử dụng

* **Frontend**: React 18, React Router, Vite.
* **Backend**: PHP 8.2, GraphQL PHP, JWT, Dotenv.
* **Realtime**: Ratchet WebSocket.
* **Database**: MySQL 8.0.
* **Container**: Docker Compose. 

### 7. Cấu trúc project

Chỉ cần nêu ở mức tổng quan:

* `frontend/`: giao diện người dùng.
* `backend/`: API, GraphQL, service, repository.
* `database/`: migration và seed.
* `deploy/`: tài liệu triển khai VPS/nginx.
* `docker-compose.yml`: chạy toàn hệ thống. 

### 8. Khả năng mở rộng

Có thể chốt bài bằng phần này:

* Thêm notification center đầy đủ.
* Mở rộng realtime ngoài chat.
* Bổ sung admin panel, rate limit, cache Redis.
* Viết test tự động và CI/CD. 

---

## Nội dung nên bỏ qua khi thuyết trình

* Toàn bộ mục **“Phân tích lỗi: Tính năng thông báo không hoạt động”**.
* Các đoạn quá chi tiết về:

  * migration cụ thể
  * command debug
  * lỗi CORS, ACK, Promise hanging
  * ghi chú cho AI model đọc code
* Bảng API quá dài nếu người nghe không phải dev backend. 

---

## Gợi ý bố cục slide

1. **Giới thiệu dự án MXH**
2. **Mục tiêu và bài toán giải quyết**
3. **Chức năng chính**
4. **Kiến trúc hệ thống**
5. **Công nghệ sử dụng**
6. **Các cập nhật nổi bật gần đây**
7. **Khả năng mở rộng trong tương lai**
8. **Kết luận**

---

## Ghi nguồn như thế nào

Bạn có thể ghi ở cuối slide hoặc cuối bài:

**Nguồn:** README dự án **MXH — Mạng xã hội (Social Network MVP)**. 

Hoặc ngắn hơn:

**Nguồn tham khảo:** Tài liệu README.md của project MXH. 

Nếu bạn muốn, mình có thể viết luôn cho bạn bản **nội dung thuyết trình 5–7 slide** ngắn gọn, sẵn để copy vào PowerPoint.
Mình lọc giúp bạn phần **nên đưa vào thuyết trình**, **bỏ qua phần lỗi**, và kèm **nguồn** như sau.

## Nội dung nên giữ để thuyết trình

### 1. Giới thiệu dự án

* **MXH** là một ứng dụng mạng xã hội dạng MVP, lấy cảm hứng từ Facebook.
* Hệ thống gồm **frontend React + Vite**, **backend PHP 8**, **MySQL**, và **WebSocket** cho chat thời gian thực.
* Toàn bộ có thể chạy bằng **Docker Compose**. 

### 2. Mục tiêu dự án

* Xây dựng bản demo/prototype cho các chức năng cốt lõi của mạng xã hội.
* Tách riêng **giao diện** và **API** để dễ mở rộng, bảo trì và phát triển thêm sau này. 

### 3. Các chức năng chính

Bạn nên gom thành 1 slide hoặc 2 slide:

* **Xác thực**: đăng ký, đăng nhập, JWT, Google login, quên mật khẩu.
* **Hồ sơ cá nhân**: avatar, ảnh bìa, bio, URL cá nhân.
* **Bài viết và tương tác**: tạo/sửa/xóa bài, like, comment, reaction.
* **Thông báo**: thông báo bình luận, nhắc tên, badge chưa đọc.
* **Quan hệ người dùng**: follow, kết bạn, lời mời kết bạn.
* **Chat realtime**: nhắn tin qua REST + WebSocket.
* **Tìm kiếm, stories, upload media, link preview**. 

### 4. Cập nhật nổi bật gần đây

Chỉ nên chọn vài điểm mạnh, không cần nói hết:

* **Nạp tiền qua VNPay**.
* **Trang Cài đặt tài khoản**.
* **Đăng nhập Google**.
* **Sidebar trái + mục Trò chơi**.
* **Reaction chi tiết và xem ai đã thả reaction**. 

### 5. Kiến trúc hệ thống

Nên nói ngắn gọn:

* Frontend gọi **REST/GraphQL** tới backend.
* Chat realtime dùng **WebSocket**.
* Dữ liệu lưu ở **MySQL**.
* Hệ thống đóng gói bằng **Docker Compose** nên dễ triển khai local hoặc VPS. 

### 6. Công nghệ sử dụng

* **Frontend**: React 18, React Router, Vite.
* **Backend**: PHP 8.2, GraphQL PHP, JWT, Dotenv.
* **Realtime**: Ratchet WebSocket.
* **Database**: MySQL 8.0.
* **Container**: Docker Compose. 

### 7. Cấu trúc project

Chỉ cần nêu ở mức tổng quan:

* `frontend/`: giao diện người dùng.
* `backend/`: API, GraphQL, service, repository.
* `database/`: migration và seed.
* `deploy/`: tài liệu triển khai VPS/nginx.
* `docker-compose.yml`: chạy toàn hệ thống. 

### 8. Khả năng mở rộng

Có thể chốt bài bằng phần này:

* Thêm notification center đầy đủ.
* Mở rộng realtime ngoài chat.
* Bổ sung admin panel, rate limit, cache Redis.
* Viết test tự động và CI/CD. 

---

## Nội dung nên bỏ qua khi thuyết trình

* Toàn bộ mục **“Phân tích lỗi: Tính năng thông báo không hoạt động”**.
* Các đoạn quá chi tiết về:

  * migration cụ thể
  * command debug
  * lỗi CORS, ACK, Promise hanging
  * ghi chú cho AI model đọc code
* Bảng API quá dài nếu người nghe không phải dev backend. 

---

## Gợi ý bố cục slide

1. **Giới thiệu dự án MXH**
2. **Mục tiêu và bài toán giải quyết**
3. **Chức năng chính**
4. **Kiến trúc hệ thống**
5. **Công nghệ sử dụng**
6. **Các cập nhật nổi bật gần đây**
7. **Khả năng mở rộng trong tương lai**
8. **Kết luận**

---

## Ghi nguồn như thế nào

Bạn có thể ghi ở cuối slide hoặc cuối bài:

**Nguồn:** README dự án **MXH — Mạng xã hội (Social Network MVP)**. 

Hoặc ngắn hơn:

**Nguồn tham khảo:** Tài liệu README.md của project MXH. 

Nếu bạn muốn, mình có thể viết luôn cho bạn bản **nội dung thuyết trình 5–7 slide** ngắn gọn, sẵn để copy vào PowerPoint.
