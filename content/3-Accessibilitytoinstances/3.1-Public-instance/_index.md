---
title : "Connect to Public Instance"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---
![SSMPublicinstance](/images/arc-02.png)

1. Go to [EC2 service management console](https://console.aws.amazon.com/ec2/v2/home).
    - Click on **Public Linux Instance**.
    - Click **Actions**.
    - Click **Security**.
    - Click **Modify IAM role**.
![Connect](/images/2/39.png)

2. At the Modify IAM role page.
    - Click to select **SSM-Role**.
    - Click **Create new AWS API Gateway**.
![Connect](/images/2/40.png)


3. Go to the [AWS Systems Manager service management console](https://console.aws.amazon.com/systems-manager/home)
    - Drag the left menu slider down.
    - Click **Session Manager**.
    - Click **Start Session**.
![Connect](/images/2/41.png)


4. Then select **Public Linux Instance** and click **Start session** to access the instance.
![Connect](/images/2/42.png)


5. Terminal will appear on the browser. Testing with the command ``` sudo tcpdump -nn port 22 ``` and ```sudo tcpdump ``` we will see no SSH traffic but only HTTPS traffic.
![Connect](/images/2/43.png)



 You can click terminate to end the currently connected session before proceeding to the next step.