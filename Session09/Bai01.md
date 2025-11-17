Bảng thực thể và vai trò trong hệ thống quản lý bán sách

| **Tên thực thể**                    | **Miêu tả vai trò**                                                                                                                                           |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Sách (Book)**                     | Chứa thông tin chi tiết về mỗi cuốn sách như tên sách, giá, mô tả, thể loại, năm xuất bản, ISBN, số lượng tồn. Đây là sản phẩm chính được bán trong hệ thống. |
| **Tác giả (Author)**                | Lưu thông tin về tác giả của sách như tên, năm sinh, quốc tịch, tiểu sử. Một tác giả có thể viết nhiều sách, và một sách cũng có thể có nhiều tác giả.        |
| **Khách hàng (Customer)**           | Lưu thông tin cá nhân của người mua như họ tên, email, địa chỉ, số điện thoại. Khách hàng tạo đơn hàng và thực hiện việc mua sách.                            |
| **Đơn hàng (Order)**                | Đại diện cho một lần mua hàng của khách hàng. Lưu thông tin như mã đơn, ngày đặt, khách hàng, tổng tiền, trạng thái đơn hàng (đã thanh toán, đang xử lý…).    |
| **Chi tiết đơn hàng (OrderDetail)** | Chứa thông tin chi tiết về từng sách trong đơn hàng như mã sách, số lượng, đơn giá. Một đơn hàng có nhiều dòng chi tiết.                                      |

Quan hệ giữa các thực thể (hiểu thêm)

Sách ↔ Tác giả: Quan hệ N-N (nhiều sách – nhiều tác giả).

Khách hàng ↔ Đơn hàng: 1-N (một khách hàng có nhiều đơn hàng).

Đơn hàng ↔ Chi tiết đơn hàng: 1-N (một đơn hàng gồm nhiều chi tiết).

Sách ↔ Chi tiết đơn hàng: N-1 (một chi tiết đơn hàng chỉ thuộc một sách).