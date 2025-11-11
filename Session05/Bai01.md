1. Phân biệt Actor, Object, Lifeline trong sơ đồ Sequence

Actor
Diễn viên bên ngoài bước vào sân khấu hệ thống. Actor đại diện cho người dùng hoặc hệ thống khác tương tác với hệ thống đang được mô tả. Actor không sống trong hệ thống, họ chỉ “gõ cửa” và gửi yêu cầu.

Object
Vật thể trong hệ thống, như những nhân viên trong hậu trường. Object là một phần của hệ thống, có trạng thái, có vai trò rõ ràng và nhận hoặc gửi thông điệp.

Lifeline
Sợi dây thời gian chạy dọc xuống dưới của mỗi Actor hoặc Object. Lifeline giống như vệt sáng cho thấy một nhân vật tồn tại và hoạt động tại từng thời điểm trong chuỗi tương tác. Khi có một “ô hoạt động” xuất hiện trên lifeline, nghĩa là nhân vật đang xử lý một công việc.

2. Liệt kê và mô tả vai trò từng thành phần trong sơ đồ Sequence:

Khách hàng, Website, Hệ thống thanh toán

1. Khách hàng (Actor)

Khách hàng là người khởi đầu mọi chuyện. Họ gửi yêu cầu, ví dụ đặt hàng hoặc thanh toán. Trong sơ đồ sequence, Khách hàng chỉ giao tiếp từ bên ngoài, không xử lý nghiệp vụ nội bộ.

2. Website (Object trong hệ thống)

Website giống như bộ mặt lẫn người dẫn chuyện. Nó nhận yêu cầu từ Khách hàng, kiểm tra dữ liệu, hiển thị thông tin, rồi chuyển tiếp các yêu cầu phức tạp sang Hệ thống thanh toán. Đây là đầu mối chính giúp mọi thứ diễn ra trơn tru.

3. Hệ thống thanh toán (Object hoặc Actor tùy phạm vi mô tả)

Nếu Hệ thống thanh toán nằm ngoài giải pháp của bạn, nó là một Actor bên ngoài. Nếu nằm trong hệ thống bạn đang thiết kế, nó là Object.
