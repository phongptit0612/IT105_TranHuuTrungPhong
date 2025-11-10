| Thành phần            | Kiểu          | Mô tả                                                    |
| --------------------- | ------------- | -------------------------------------------------------- |
| `orderId`             | String / int  | Mã định danh duy nhất của đơn hàng                       |
| `orderDate`           | Date          | Ngày tạo đơn hàng                                        |
| `totalAmount`         | float         | Tổng số tiền của đơn hàng                                |
| `productList`         | List<Product> | Danh sách sản phẩm trong đơn hàng                        |
| `addProduct(product)` | Method        | Thêm một sản phẩm vào đơn hàng                           |
| `calculateTotal()`    | Method        | Tính tổng số tiền của đơn hàng dựa trên các sản phẩm     |
| `checkout()`          | Method        | Thực hiện đặt đơn hàng và cập nhật trạng thái thanh toán |

//Dang txt
Class Order
------------------------
+ orderId
+ orderDate
+ totalAmount
+ productList
------------------------
+ addProduct(product)
+ calculateTotal()
+ checkout()
