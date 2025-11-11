1. Phân loại các loại thông điệp
(1) Khách hàng gửi yêu cầu đăng nhập đến Website

Loại: Synchronous Message

Lý do: Website phải nhận và xử lý trước khi có bước tiếp theo. Khách hàng không thể tiếp tục cho đến khi website phản hồi.

(2) Website gửi thông tin xác minh đến Hệ thống xác minh

Loại: Synchronous Message

Lý do: Website phải chờ kết quả xác minh để quyết định trả về giao diện cá nhân hay báo lỗi.

(3) Hệ thống xác minh trả kết quả cho Website

Loại: Return Message

Lý do: Đây là phản hồi của thao tác xác minh thông tin.

(4) Website trả giao diện cá nhân cho Khách hàng

Loại: Return Message

Lý do: Đây là kết quả cho yêu cầu đăng nhập ban đầu.

2. Có Asynchronous Message hay không?

Trong quy trình đăng nhập chuẩn như mô tả, không có asynchronous message.
Vì cả Website và Hệ thống xác minh đều phải chờ kết quả của nhau. Việc xác minh danh tính không thể chạy song song hoặc bỏ ngỏ.

Tuy vậy, trong các hệ thống lớn, bên trong có thể xuất hiện async như “ghi log”, “gửi email”, nhưng quy trình bạn mô tả thì không dùng.