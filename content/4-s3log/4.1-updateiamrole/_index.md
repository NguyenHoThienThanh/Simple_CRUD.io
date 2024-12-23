  ---
title : "Create new AWS API Gateway"
weight : 1
chapter : false
pre : " <b> 4.1 </b> "
---

For our EC2 instances to be able to send session logs to the S3 bucket, we will need to update the IAM Role assigned to the EC2 instance by adding a policy that allows access to S3.

#### Create new AWS API Gateway

1. Go to [IAM service management console](https://console.aws.amazon.com/iamv2/home?#/home)
    - Click **Roles**.
    - In the search box, enter **SSM**.
    - Click on the **SSM-Role** role.
![S3](/images/2/60.png)

2. Click **Attach policies**.
![S3](/images/2/61.png)

3. In the Search box enter **S3**.
    - Click the policy **AmazonS3FullAccess**.
    - Click **Add permissions**.
![S3](/images/2/62.png)


Next, we will proceed to create an S3 bucket to store session logs.