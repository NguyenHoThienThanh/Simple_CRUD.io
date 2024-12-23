---
title : "Giới thiệu"
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---
## Giới Thiệu

Trong thế giới điện toán đám mây hiện nay, kiến trúc serverless (không máy chủ) đang ngày càng được ưa chuộng nhờ khả năng mở rộng, hiệu quả chi phí và dễ dàng bảo trì. Dự án này sẽ hướng dẫn cách xây dựng một API CRUD (Tạo, Đọc, Cập nhật, Xóa) đơn giản bằng **AWS Lambda**, **API Gateway** và **MongoDB**. Những công nghệ này cung cấp các công cụ mạnh mẽ để phát triển các ứng dụng web có thể mở rộng và tiết kiệm chi phí với ít sự can thiệp từ người quản trị.

### AWS Lambda là gì?

AWS Lambda là một dịch vụ điện toán không máy chủ giúp tự động quản lý tài nguyên tính toán cần thiết để chạy mã của bạn khi có sự kiện xảy ra. Với Lambda, bạn không cần phải cung cấp hoặc quản lý máy chủ, điều này làm cho nó trở thành một lựa chọn lý tưởng để xây dựng các microservices và API trong môi trường có khả năng mở rộng cao.

### API Gateway là gì?

AWS API Gateway là một dịch vụ quản lý hoàn toàn cho phép các nhà phát triển tạo và xuất bản các API RESTful cho các dịch vụ backend. Nó hoạt động như một cổng cho các yêu cầu HTTP, kết nối các client với các hàm AWS Lambda, giúp quản lý API một cách an toàn và có khả năng mở rộng cao.

### Tại sao chọn MongoDB?

MongoDB là một cơ sở dữ liệu NoSQL cung cấp sự linh hoạt và khả năng mở rộng. Đây là lựa chọn lý tưởng cho các ứng dụng yêu cầu phát triển nhanh chóng và khả năng mở rộng cao. Trong dự án này, MongoDB sẽ được sử dụng để lưu trữ dữ liệu mà API CRUD xử lý, giúp ứng dụng có thể quản lý khối lượng dữ liệu và lưu lượng truy cập lớn một cách hiệu quả.

### Mục Tiêu

Mục tiêu của dự án này là hướng dẫn bạn cách xây dựng một API CRUD đơn giản, giúp:

1. Cho phép các client tương tác với dữ liệu lưu trữ trong cơ sở dữ liệu MongoDB.
2. Sử dụng các hàm AWS Lambda cho từng thao tác CRUD, đảm bảo API không có máy chủ và có thể mở rộng.
3. Sử dụng AWS API Gateway để định tuyến các yêu cầu HTTP và tương tác an toàn với các hàm Lambda.

Cuối cùng, bạn sẽ có một API serverless hoàn chỉnh có khả năng xử lý các tác vụ quản lý dữ liệu mà không cần phải quản lý cơ sở hạ tầng hoặc lo lắng về việc mở rộng.
