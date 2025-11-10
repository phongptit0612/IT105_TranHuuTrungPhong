| Thành phần        | Modifier  | Giải thích                                                                                                        |
| ----------------- | --------- | ----------------------------------------------------------------------------------------------------------------- |
| `username`        | `public`  | Tên người dùng có thể được truy cập từ bên ngoài, ví dụ hiển thị trong giao diện hoặc báo cáo.                    |
| `password`        | `private` | Mật khẩu cần bảo mật, không để đối tượng bên ngoài truy cập trực tiếp. Chỉ truy cập thông qua phương thức hợp lệ. |
| `login()`         | `public`  | Phương thức đăng nhập phải được gọi từ bên ngoài, ví dụ từ giao diện người dùng.                                  |
| `resetPassword()` | `public`  | Cho phép người dùng hoặc hệ thống gọi để đặt lại mật khẩu. Có thể có kiểm tra bảo mật bên trong.                  |
| `lastLoginTime`   | `private` | Thời gian đăng nhập cuối cùng không nên thay đổi trực tiếp từ bên ngoài, chỉ truy cập thông qua getter nếu cần.   |
