| Mã hóa đơn | Tên khách hàng | Số điện thoại | Danh sách sản phẩm | Tổng tiền |
| ---------- | -------------- | ------------- | ------------------ | --------- |
| HD001      | An             | 0912345678    | Bút bi, Vở, Thước  | 50,000    |
| HD002      | Bình           | 0987654321    | Sách, Bút chì      | 80,000    |

 Vấn đề:

Cột "Danh sách sản phẩm" chứa nhiều giá trị trong một ô → vi phạm 1NF.

Thông tin khách hàng lặp lại → dư thừa.

Không tách rõ đơn hàng – sản phẩm → khó quản lý chi tiết đơn hàng.

Chuẩn hóa 1NF (First Normal Form): Bảng Hóa Đơn 1NF (Order_1NF)

| Mã hóa đơn (PK) | Tên khách hàng | Số điện thoại | Sản phẩm | Tổng tiền |
| --------------- | -------------- | ------------- | -------- | --------- |
| HD001           | An             | 0912345678    | Bút bi   | 50,000    |
| HD001           | An             | 0912345678    | Vở       | 50,000    |
| HD001           | An             | 0912345678    | Thước    | 50,000    |
| HD002           | Bình           | 0987654321    | Sách     | 80,000    |
| HD002           | Bình           | 0987654321    | Bút chì  | 80,000    |

Chuẩn hóa 2NF (Second Normal Form): Bảng Hóa Đơn (Orders)

| Mã hóa đơn (PK) | Tên khách hàng | Số điện thoại | Tổng tiền |
| --------------- | -------------- | ------------- | --------- |
| HD001           | An             | 0912345678    | 50,000    |
| HD002           | Bình           | 0987654321    | 80,000    |

Bảng Chi Tiết Hóa Đơn (OrderDetails)

| Mã hóa đơn (FK) | Sản phẩm |
| --------------- | -------- |
| HD001           | Bút bi   |
| HD001           | Vở       |
| HD001           | Thước    |
| HD002           | Sách     |
| HD002           | Bút chì  |

Chuẩn hóa 3NF (Third Normal Form):

Bảng Khách Hàng (Customer)
| CustomerID (PK) | Tên khách hàng | Số điện thoại |
| --------------- | -------------- | ------------- |
| C001            | An             | 0912345678    |
| C002            | Bình           | 0987654321    |

Bảng Hóa Đơn (Orders)
| Mã hóa đơn (PK) | CustomerID (FK) | Tổng tiền |
| --------------- | --------------- | --------- |
| HD001           | C001            | 50,000    |
| HD002           | C002            | 80,000    |

Bảng Chi Tiết Hóa Đơn (OrderDetails)
| OrderDetailID (PK) | Mã hóa đơn (FK) | Sản phẩm |
| ------------------ | --------------- | -------- |
| 1                  | HD001           | Bút bi   |
| 2                  | HD001           | Vở       |
| 3                  | HD001           | Thước    |
| 4                  | HD002           | Sách     |
| 5                  | HD002           | Bút chì  |
