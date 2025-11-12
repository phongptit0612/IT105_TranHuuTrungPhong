1. Nhận biết loại hệ thống thông tin phù hợp

Dựa vào các chức năng:
Cập nhật đơn hàng → Xử lý dữ liệu giao dịch theo thời gian thực.
Theo dõi trạng thái → Giám sát hoạt động, báo cáo tiến trình.
Phân tích tuyến đường → Hỗ trợ ra quyết định, tối ưu hóa quy trình vận chuyển.
Ta có thể phân loại các hệ thống như sau:

| Tính năng                    | Loại hệ thống phù hợp                   | Lý do                                                                                                              |
| ---------------------------- | --------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Cập nhật đơn hàng            | **TPS (Transaction Processing System)** | Xử lý các giao dịch hàng ngày: tạo đơn, cập nhật trạng thái, thanh toán, yêu cầu thời gian thực, chính xác.        |
| Theo dõi trạng thái          | **MIS (Management Information System)** | Tổng hợp dữ liệu từ TPS, cung cấp báo cáo và thống kê cho quản lý theo dõi tiến trình đơn hàng.                    |
| Phân tích tuyến đường        | **DSS (Decision Support System)**       | Hỗ trợ ra quyết định: phân tích dữ liệu, tối ưu hóa tuyến đường giao hàng, dự báo thời gian và chi phí vận chuyển. |
| Báo cáo cấp cao cho lãnh đạo | **EIS (Executive Information System)**  | Cung cấp thông tin tổng quan, KPI, báo cáo hiệu suất vận hành cho ban lãnh đạo.                                    |

2. Mô hình phát triển phần mềm thích hợp

Phân tích yêu cầu:
Hệ thống liên quan đến giao dịch trực tuyến và dữ liệu thời gian thực → cần độ chính xác và bảo mật cao.
Cần phản hồi người dùng thường xuyên (cập nhật trạng thái, theo dõi, báo cáo) → yêu cầu linh hoạt, có khả năng thay đổi yêu cầu trong quá trình phát triển.
Tính năng tối ưu hóa tuyến đường có thể cần cải tiến dựa trên dữ liệu thực tế → yêu cầu mô hình phát triển thích ứng nhanh.
Đánh giá các mô hình:

       Mô hình	                                        Ưu điểm trong trường hợp này	                                                   Nhược điểm
Waterfall (Thác nước) ||	Rõ ràng, tuần tự; thích hợp với yêu cầu ổn định, dễ kiểm soát || Khó thay đổi khi yêu cầu thay đổi; không linh hoạt với các tính năng tối ưu tuyến đường cần cải tiến liên tục
Agile / Scrum   ||    Linh hoạt, cải tiến liên tục; phù hợp phát triển các tính năng theo module (đơn hàng, theo dõi, DSS)   ||    Cần đội ngũ phản hồi nhanh và quản lý sprint hiệu quả
Incremental / Iterative  ||   Phát triển theo từng phần, có thể triển khai TPS trước, DSS sau   ||   Cần kế hoạch tích hợp chặt chẽ, nếu thiếu có thể gây trễ tổng thể