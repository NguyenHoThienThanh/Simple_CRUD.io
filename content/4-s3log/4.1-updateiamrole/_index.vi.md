---
title : "Cập nhật IAM Role"
weight : 1 
chapter : false
pre : " <b> 4.1 </b> "
---

Để các EC2 instance của chúng ta có thể gửi session log tới S3 bucket , chúng ta sẽ cần cập nhật IAM Role đã gán vào EC2 instance bằng cách thêm vào policy cho phép quyền truy cập vào S3.

#### Cập nhật IAM Role

1. Truy cập vào [giao diện quản trị dịch vụ IAM](https://console.aws.amazon.com/iamv2/home?#/home)
    - Click **Roles**.
    - Tại ô tìm kiếm , điền **SSM**.
    - Click vào role **SSM-Role**.
![S3](/images/2/60.png)

2. Click **Attach policies**.
![S3](/images/2/61.png)

3. Tại ô Search điền **S3**.
    - Click chọn policy **AmazonS3FullAccess**.
    - Click **Add permissions**.
![S3](/images/2/62.png)


Tiếp theo chúng ta sẽ tiến hành tạo S3 bucket để lưu trữ session logs.