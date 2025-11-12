1. Xác định Stakeholders
| Stakeholder                                  | Vai trò trong hệ thống                          | Nguồn yêu cầu                               |
| -------------------------------------------- | ----------------------------------------------- | ------------------------------------------- |
| Học viên (Students)                          | Người dùng cuối, mua và học khóa học trực tuyến | Người dùng cuối, nhu cầu học tập trực tuyến |
| Giảng viên (Instructors)                     | Tạo và quản lý khóa học, theo dõi học viên      | Người tạo nội dung, giáo viên               |
| Quản trị viên (Admin)                        | Quản lý hệ thống, giám sát người dùng, báo cáo  | Ban quản lý, yêu cầu vận hành hệ thống      |
| Nhân viên hỗ trợ (Support Staff)             | Hỗ trợ học viên và giảng viên khi gặp sự cố     | Yêu cầu dịch vụ khách hàng                  |
| Bộ phận marketing (Marketing)                | Quảng bá khóa học, thu hút học viên             | Chiến lược kinh doanh                       |
| Bộ phận thanh toán (Finance/Payment Gateway) | Xử lý thanh toán và giao dịch                   | Yêu cầu kinh doanh và pháp lý               |
| Nhà cung cấp nội dung (Content Providers)    | Cung cấp tài liệu, video, bài giảng             | Nguồn nội dung bên ngoài                    |
| Hệ thống IT/DevOps                           | Duy trì vận hành, bảo trì, nâng cấp hệ thống    | Yêu cầu kỹ thuật, bảo mật và hiệu suất      |
| Ban lãnh đạo (Management)                    | Ra quyết định, đánh giá hiệu quả kinh doanh     | Mục tiêu chiến lược và KPI                  |


2. Phân tích yêu cầu của hệ thống E-learning

 2.1 Yêu cầu chức năng (Functional Requirements)

| ID   | Yêu cầu chức năng          | Mô tả chi tiết                                                                           |
| ---- | -------------------------- | ---------------------------------------------------------------------------------------- |
| FR1  | Đăng ký và đăng nhập       | Học viên và giảng viên có thể tạo tài khoản và đăng nhập bằng email/social media.        |
| FR2  | Quản lý hồ sơ người dùng   | Người dùng có thể xem và chỉnh sửa thông tin cá nhân.                                    |
| FR3  | Tìm kiếm và duyệt khóa học | Học viên có thể tìm khóa học theo chủ đề, mức độ, giảng viên, giá cả.                    |
| FR4  | Mua khóa học               | Học viên có thể thêm khóa học vào giỏ và thanh toán online.                              |
| FR5  | Xem nội dung khóa học      | Học viên có thể xem video, tài liệu, bài kiểm tra trong khóa học đã mua.                 |
| FR6  | Quản lý khóa học           | Giảng viên có thể tạo, chỉnh sửa, xóa khóa học, upload nội dung, quản lý bài kiểm tra.   |
| FR7  | Theo dõi tiến độ học tập   | Học viên có thể theo dõi tiến độ khóa học, hoàn thành bài tập.                           |
| FR8  | Hệ thống thông báo         | Gửi thông báo về khóa học mới, nhắc nhở học viên, cập nhật từ giảng viên.                |
| FR9  | Báo cáo và thống kê        | Admin và giảng viên có thể xem báo cáo về số lượng học viên, doanh thu, tiến độ học tập. |
| FR10 | Hỗ trợ trực tuyến          | Học viên và giảng viên có thể gửi yêu cầu hỗ trợ và nhận phản hồi từ bộ phận hỗ trợ.     |

 2.2 Yêu cầu phi chức năng (Non-functional Requirements)

| ID   | Yêu cầu phi chức năng                    | Mô tả chi tiết                                                                            |
| ---- | ---------------------------------------- | ----------------------------------------------------------------------------------------- |
| NFR1 | Hiệu suất (Performance)                  | Hệ thống có thể phục vụ đồng thời 10.000+ người dùng mà không giảm tốc độ.                |
| NFR2 | Bảo mật (Security)                       | Dữ liệu người dùng, thanh toán được mã hóa; có cơ chế chống tấn công DDoS, SQL Injection. |
| NFR3 | Khả năng mở rộng (Scalability)           | Hệ thống dễ dàng mở rộng khi số lượng người dùng tăng.                                    |
| NFR4 | Tính sẵn sàng (Availability)             | Hệ thống hoạt động 24/7, thời gian downtime < 1%/năm.                                     |
| NFR5 | Tính khả dụng (Usability)                | Giao diện thân thiện, dễ sử dụng trên web và mobile.                                      |
| NFR6 | Tính tương thích (Compatibility)         | Hỗ trợ các trình duyệt phổ biến, thiết bị di động và desktop.                             |
| NFR7 | Bảo trì (Maintainability)                | Hệ thống dễ bảo trì, nâng cấp mà không ảnh hưởng lớn đến người dùng.                      |
| NFR8 | Khả năng phục hồi (Recovery)             | Hệ thống có backup dữ liệu tự động và khôi phục nhanh khi xảy ra sự cố.                   |
| NFR9 | Hiệu quả thanh toán (Payment efficiency) | Thanh toán phải được xử lý nhanh, xác nhận tức thì cho học viên.                          |
