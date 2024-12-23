---
title : "Tạo S3 Bucket" 
weight : 2 
chapter : false
pre : " <b> 4.2 </b> "
---


Trong bước này, chúng ta sẽ tạo 1 S3 bucket để lưu trữ các session logs được gửi từ các EC2 instance.

#### Tạo **S3 Bucket**

1. Truy cập [giao diện quản trị dịch vụ S3](https://s3.console.aws.amazon.com/s3/home)
    - Click **Create bucket**.
![S3](/images/2/63.png)

2. Tại trang **Create bucket**.
    - In the **Bucket type**, select **General purpose**
    - Tại mục **Bucket name** điền tên bucket **lab-yourname-bucket-0001**
    - In the **Object Ownership** section, select **ACLs disable (recommended)**
![S3](/images/2/64.png)



3. Kéo chuột xuống phía dưới và click **Create bucket**.
![S3](/images/2/65.png)


