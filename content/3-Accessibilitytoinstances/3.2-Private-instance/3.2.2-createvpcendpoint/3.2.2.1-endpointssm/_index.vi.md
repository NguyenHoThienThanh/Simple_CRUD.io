---
title : "Tạo Endpoint ssm"
weight : 1
chapter : false
pre : " <b> 3.2.2.1 </b> "
---


#### Tải AWS CLI Endpoint SSM

1. Truy cập đến [giao diện quản trị của dịch vụ VPC](https://console.aws.amazon.com/vpc/home)
    - Click **Endpoints**.
    - Click **Create endpoint**.
![Connect](/images/2/46.png)

2. Tại trang **Create endpoint**.
    - Tại mục **Name tag** điền **SSM**.
    - Tại mục **Service Category** chọn **AWS Services**.
    - Tại mục **Service**, điền ```.ssm``` vào thanh tìm kiếm
    - Tại mục **Service category** chọn:  **AWS services**
      - Sau đó chọn **Service Name: com.amazonaws.ap-southeast-1.ssm**.
![Connect](/images/2/47.png)

3.  - Tại mục **VPC**, chọn **Lab VPC**.
    - Chọn AZ đầu tiên, sau đó chọn subnet **Lab Private Subnet**.
![Connect](/images/2/48.png)

4. Kéo chuột xuống dưới.
    - Tại mục **Security Group**, chọn Security group **SG VPC Endpoint** mà chúng ta đã tạo trước đó.
    - Tại mục **Policy**, chọn **Full access**
![Connect](/images/2/49.png)

5. Kéo chuột xuống dưới cùng.
    - Click **Create endpoint**.

6. Chúng ta đã tạo xong VPC Interface Endpoint cho **SSM**.