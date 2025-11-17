| **Entity**        | **Attribute**        | **Kiểu dữ liệu**                      | **Vai trò**                                       |
| ----------------- | -------------------- | ------------------------------------- | ------------------------------------------------- |
| **User**          | UserID               | INT (PK)                              | Định danh duy nhất cho mỗi người dùng             |
|                   | FullName             | VARCHAR(100)                          | Lưu tên đầy đủ của người dùng                     |
|                   | Email                | VARCHAR(100)                          | Dùng để đăng nhập, xác định tài khoản             |
|                   | Role                 | ENUM('student','teacher')             | Xác định người dùng là học viên hay giảng viên    |
|                   | CreatedAt            | DATETIME                              | Thời gian tài khoản được tạo                      |
| ----------------- | -------------------- | ------------------                    | -------------                                     |
| **Course**        | CourseID             | INT (PK)                              | Định danh duy nhất cho mỗi khóa học               |
|                   | Title                | VARCHAR(150)                          | Tên khóa học                                      |
|                   | Description          | TEXT                                  | Mô tả nội dung khóa học                           |
|                   | Price                | DECIMAL(10,2)                         | Học phí khóa học                                  |
|                   | TeacherID            | INT (FK)                              | Liên kết đến User (giảng viên) giảng dạy khóa học |
| ----------------- | -------------------- | ------------------                    | -------------                                     |
| **Enrollment**    | EnrollmentID         | INT (PK)                              | Định danh duy nhất cho mỗi lượt đăng ký           |
|                   | UserID               | INT (FK)                              | Người dùng đăng ký khóa học                       |
|                   | CourseID             | INT (FK)                              | Khóa học mà người dùng đăng ký                    |
|                   | EnrollDate           | DATETIME                              | Thời gian đăng ký khóa học                        |
|                   | Status               | ENUM('active','completed','canceled') | Trạng thái đăng ký                                |
