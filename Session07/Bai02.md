Mô tả chi tiết từng tầng
Tầng 1: Presentation Tier (Tầng giao diện)

Vai trò:

Là nơi người dùng tương tác với hệ thống (Web App hoặc Mobile App)

Hiển thị màn hình quản lý sản phẩm, nhà cung cấp và nhập–xuất kho

Gửi yêu cầu đến tầng Business thông qua các controller

Thành phần:

UI (HTML/CSS/JS hoặc Mobile UI)

Controller: nhận request, validate dữ liệu, gọi các service

Ví dụ:

Trang thêm sản phẩm

Màn hình xem tồn kho

Form nhập hàng, xuất hàng

Tầng 2: Business Logic Tier (Tầng xử lý nghiệp vụ)

Vai trò:
Xử lý các logic chính của hệ thống:

ProductService

Thêm / sửa / xóa sản phẩm

Kiểm tra tính hợp lệ mã sản phẩm

Kiểm tra trùng tên hoặc trùng mã

SupplierService

Lưu thông tin nhà cung cấp

Xử lý đơn hàng nhập từ nhà cung cấp

InventoryService

Xử lý logic nhập – xuất kho

Cập nhật tồn kho (quantity_in_stock)

Tính toán số lượng khả dụng

Ngăn chặn xuất kho khi không đủ hàng

Đặc điểm:

Tầng này không biết cách dữ liệu được lưu như thế nào

Chỉ gọi Repository để lấy/ghi dữ liệu
Tầng 3: Data Access Tier (Tầng truy cập dữ liệu)

Vai trò:

Tương tác trực tiếp với CSDL (MySQL, PostgreSQL, …)

Cung cấp CRUD cho Business Tier

Thành phần:

ProductRepository

save(product)

findById(id)

delete(id)

SupplierRepository

Lưu/truy vấn thông tin nhà cung cấp

InventoryRepository

Lưu LOG nhập – xuất kho

Update tồn kho