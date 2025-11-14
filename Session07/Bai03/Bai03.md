Mô tả từng Module:

Flight Search Module – Tìm chuyến bay

Chịu trách nhiệm cung cấp thông tin chuyến bay từ dữ liệu hãng hàng không.

Thành phần:

FlightSearchService: xử lý yêu cầu tìm chuyến bay theo ngày, điểm đi, điểm đến

FlightFilter: lọc chuyến theo giá, giờ bay, hãng bay

FlightRepository: truy vấn dữ liệu chuyến bay từ database hoặc API hãng bay

Luồng: Người dùng nhập thông tin → module trả danh sách chuyến bay hợp lệ.

Booking Module – Đặt vé

Xử lý toàn bộ quá trình đặt vé trước khi thanh toán.

Thành phần:

BookingService: quy trình đặt vé (chọn chuyến → chọn ghế → nhập hành khách)

SeatSelection: kiểm tra ghế trống và gán ghế

PassengerInfo: lưu thông tin hành khách

BookingRepository: lưu thông tin đặt chỗ tạm thời

Luồng: Người dùng chọn chuyến → nhập thông tin → giữ chỗ.

Payment Module – Thanh toán

Quản lý quy trình thanh toán và xuất hóa đơn.

Thành phần:

PaymentService: xử lý nghiệp vụ thanh toán

PaymentGatewayAdapter: tích hợp MoMo, VNPay, PayPal…

InvoiceGenerator: tạo hóa đơn điện tử

PaymentRepository: lưu giao dịch thanh toán

Luồng: Sau khi đặt chỗ → thanh toán → xác nhận → gửi email.


Account Module – Quản lý tài khoản

Xử lý tính năng đăng ký, đăng nhập, hồ sơ người dùng.

Thành phần:

UserService: quản lý thông tin người dùng

Authentication: đăng nhập, JWT/OAuth2

UserProfile: thông tin cá nhân

UserRepository: lưu dữ liệu tài khoản

Luồng: User đăng nhập → truy cập vào lịch sử vé, thông tin cá nhân.

Mối liên kết giữa các Module

Booking → dùng Flight Search để kiểm tra chuyến

Booking → gọi Payment để xử lý thanh toán

Account → được dùng để xác thực khi đặt vé hoặc thanh toán