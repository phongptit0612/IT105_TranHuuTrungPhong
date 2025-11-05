1. Planning (Lập kế hoạch)

Mục tiêu: Xây dựng hệ thống giúp giảng viên điểm danh nhanh, sinh viên tự quét QR, phòng đào tạo quản lý dữ liệu tập trung.

Phạm vi: Ứng dụng mobile + web quản trị.

Nguồn lực:

Nhóm phát triển phần mềm (backend, mobile, UI/UX)

Thiết bị: máy chủ, smartphone, mạng nội bộ trường

Kế hoạch:

Thời gian: 3 tháng

Giai đoạn: phân tích → thiết kế → lập trình → kiểm thử → triển khai thử nghiệm

 2. Requirement Analysis (Phân tích yêu cầu)

Người dùng chính:

Giảng viên: tạo buổi học, hiển thị mã QR, xem danh sách sinh viên điểm danh.

Sinh viên: đăng nhập và quét mã QR để điểm danh.

Phòng đào tạo: xem thống kê, xuất báo cáo điểm danh.

Yêu cầu chức năng:

Đăng nhập theo vai trò (GV, SV, Phòng đào tạo)

Tạo buổi học + sinh mã QR duy nhất

Quét mã QR để xác nhận điểm danh

Lưu trữ dữ liệu điểm danh theo lớp và buổi học

Xuất thống kê báo cáo

Yêu cầu phi chức năng:

Bảo mật dữ liệu sinh viên

Tốc độ phản hồi nhanh

Giao diện thân thiện

3. System Design (Thiết kế hệ thống)

Thiết kế kiến trúc:

Ứng dụng mobile (cho sinh viên và giảng viên) kết nối server backend qua API.

CSDL trung tâm lưu thông tin người dùng, buổi học, điểm danh.

Thiết kế dữ liệu:

Bảng Users, Classes, Sessions, AttendanceRecords.

Thiết kế giao diện:

Màn hình đăng nhập, quét QR, tạo buổi học, xem thống kê.

Thiết kế UML sơ bộ:

Use Case Diagram: mô tả 3 tác nhân (Giảng viên, Sinh viên, Phòng đào tạo) và các chức năng tương ứng.

Class Diagram: thể hiện mối quan hệ giữa lớp User, Class, Session, Attendance.

Sequence Diagram: mô tả luồng “Sinh viên quét mã QR → hệ thống xác nhận điểm danh”.