1. Khi nào dùng include, khi nào dùng extend?

include

Dùng khi một use case luôn luôn cần thực hiện một use case khác để hoàn thành.

Giống như việc bạn luôn phải mở khóa cửa trước khi bước vào nhà.

Tính chất: bắt buộc, lặp đi lặp lại ở nhiều nơi.

extend

Dùng khi một use case có thể thêm bước mở rộng tùy tình huống.

Giống như thỉnh thoảng bạn mới bật đèn sân khi về nhà buổi tối.

Tính chất: tùy chọn, chỉ xảy ra trong điều kiện đặc biệt.

2. Xác định quan hệ giữa 4 Use Case

Use case bạn đưa ra thuộc lĩnh vực mua hàng online. Ta có thể suy luận:

Đặt hàng thường cần Kiểm tra giỏ hàng trước. Đây là hành vi bắt buộc. → include

Xem đánh giá chỉ là hành vi tùy chọn người dùng có thể thực hiện trong khi mua sắm, không bắt buộc để đặt hàng. Thường nó là kịch bản mở rộng. → extend

Đề xuất hóa đơn có thể xuất hiện sau khi đặt hàng hoàn tất, như gợi ý thêm dịch vụ/hoá đơn. Không bắt buộc. → extend



| Use Case A        | Use Case B        | Mối quan hệ | Giải thích                                                                                            |
| ----------------- | ----------------- | ----------- | ----------------------------------------------------------------------------------------------------- |
| Đặt hàng          | Kiểm tra giỏ hàng | include     | Để đặt hàng, người dùng luôn phải kiểm tra và xác nhận giỏ hàng.                                      |
| Đặt hàng          | Xem đánh giá      | extend      | Người dùng có thể xem đánh giá khi xem sản phẩm, nhưng không bắt buộc trong quá trình đặt hàng.       |
| Đặt hàng          | Đề xuất hóa đơn   | extend      | Sau khi đặt hàng, hệ thống có thể gợi ý hóa đơn hoặc dịch vụ thêm, nhưng chỉ xuất hiện tùy điều kiện. |
| Kiểm tra giỏ hàng | Xem đánh giá      | association | Hai hành động liên quan trong bối cảnh mua sắm nhưng không phụ thuộc nhau.                            |
| Xem đánh giá      | Đề xuất hóa đơn   | association | Không phụ thuộc; chỉ là các chức năng độc lập trong hệ thống.                                         |
