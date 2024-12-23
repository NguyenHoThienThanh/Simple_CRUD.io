---
title : "Configure AWS API Gateway"
weight : 2
chapter : false
pre : " <b> 4.2 </b> "
---


In this step, we will create an S3 bucket to store session logs sent from EC2 instances.

#### Create **S3 Bucket**

1. Access [S3 service management console](https://s3.console.aws.amazon.com/s3/home)
    - Click **Create bucket**.
![S3](/images/2/63.png)

2. At the **Create bucket** page.
    - In the **Bucket type**, select **General purpose**
    - In the **Bucket name** field, enter the bucket name **lab-yourname-bucket-0001**
    - In the **Object Ownership** section, select **ACLs disable (recommended)**
![S3](/images/2/64.png)

 

3. Scroll down and click **Create bucket**.
![S3](/images/2/65.png)

