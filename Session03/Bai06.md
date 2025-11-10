USE CASE DESCRIPTION – ĐĂNG NHẬP

Tên Use Case: Đăng nhập

Actor:

Người dùng (User) – Primary actor

Hệ thống – Secondary actor

Mục tiêu:
Người dùng đăng nhập vào hệ thống để sử dụng các chức năng và dịch vụ được cấp quyền.

Luồng chính (Main Flow)

Người dùng chọn chức năng “Đăng nhập”.

Hệ thống hiển thị giao diện đăng nhập.

Người dùng nhập tên đăng nhập và mật khẩu.

Hệ thống kiểm tra thông tin đăng nhập.

Nếu thông tin hợp lệ, hệ thống cho phép người dùng truy cập.

Hệ thống chuyển người dùng đến màn hình chính.

Luồng lỗi (Exception Flow)
E1 – Sai mật khẩu / sai tên đăng nhập

3a. Người dùng nhập sai tên đăng nhập hoặc mật khẩu.
4a. Hệ thống thông báo “Thông tin đăng nhập không chính xác”.
4b. Hệ thống yêu cầu nhập lại.
→ Quay lại bước 3 của Luồng chính.

E2 – Tài khoản bị khóa

4c. Hệ thống phát hiện tài khoản đang bị khóa.
4d. Hệ thống thông báo: “Tài khoản đã bị khóa, vui lòng liên hệ hỗ trợ”.
→ Kết thúc Use Case.

E3 – Hệ thống lỗi / mất kết nối

4e. Hệ thống không thể kiểm tra thông tin do lỗi kỹ thuật.
4f. Hệ thống thông báo “Không thể xử lý, vui lòng thử lại sau”.
→ Kết thúc Use Case.