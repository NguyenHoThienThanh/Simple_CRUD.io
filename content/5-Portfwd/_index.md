---
title : "Create AWS API Gateway"
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---


We will configure **Create AWS API Gateway** for the RDP connection between our machine and **Private Windows Instance** located in the private subnet we created for this exercise.

![port-fwd](/images/arc-04.png) 

#### Create IAM user with permission to connect SSM

1. Go to [IAM service management console](https://console.aws.amazon.com/iamv2/home)
   - Click **Users** , then click **Create users**.
![FWD](/images/2/74.png)

2. At the **Create user** page.
   - In the **User name** field, enter **Portfwd**.
   - Click **Next**.
![FWD](/images/2/75.png)

3. At the **Set permission** page
   - Select **Attach policies directly**
   - In the search box, enter **ssm**.
   - Click on **AmazonSSMFullAccess**.
   - Click **Next**, click **Next: Reviews**.
   - Click **Create user**.
![FWD](/images/2/76.png)
4. Create access key for **Portfwd** user 
   - Click **Create access key**
   ![FWD](/images/2/77.png)
   - Select **Command Line Interface(CLI)**
   - Check box confirmation
   - Click **Next**
![FWD](/images/2/78.png)
   - Click **Download.csv file**
![FWD](/images/2/79.png)

Save **Access key ID** and **Secret access key** information to perform AWS CLI configuration.
#### Install and Configure AWS CLI and Session Manager Plugin
  
To perform this hands-on, make sure your workstation has [AWS CLI]() and [Session Manager Plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session) installed -manager-working-with-install-plugin.html)

More hands-on tutorials on installing and configuring the AWS CLI can be found [here](https://000011.awsstudygroup.com/).



#### Implement Portforwarding

1. Run the command below in **Command Prompt** on your machine to configure **Create AWS API Gateway**.
   ```
      aws ssm start-session --target (your ID windows instance) --document-name AWS-StartPortForwardingSession --parameters portNumber="3389",localPortNumber="9999" --region (your region)
   ```


   - Example command:
   ```
   C:\Windows\system32>aws ssm start-session --target i-06343d7377486760c --document-name AWS-StartPortForwardingSession --parameters portNumber="3389",localPortNumber="9999" --region us-east-1
   ```

 

2. Connect to the **Private Windows Instance** you created using the **Remote Desktop** tool on your workstation.
   - In the Computer section: enter **localhost:9999**.
![FWD](/images/2/80.png)

3. Return to the administration interface of the System Manager - Session Manager service.
   - Click tab **Session history**.
   - We will see session logs with Document name **AWS-StartPortForwardingSession**.
![FWD](/images/2/81.png)


Congratulations on completing the lab on how to use Session Manager to connect and store session logs in S3 bucket. Remember to perform resource cleanup to avoid unintended costs.