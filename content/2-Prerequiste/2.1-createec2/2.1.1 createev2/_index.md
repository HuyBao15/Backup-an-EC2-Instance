---
title : "Create EC2"
date : "2024-12-05"
weight : 1
chapter : false
pre : " <b> 2.1.1 </b> "
---


#### Create EC2 
1. Go to [AWS Management Console](https://aws.amazon.com/console/) and open **AWS EC2 Console**
   + Click **EC2**
![EC2](/images/2.prerequisite/01-openec2.png)


2. In the navigation pane on the left side of the **AWS EC2 console**, under **Intances**, choose **Intances**, then choose **Launch Instance**.
![EC2](/images/2.prerequisite/02-openinstances.png)

- On the **Launch an instance** page, under the **Name** section, enter name for your instance.
![EC2](/images/2.prerequisite/03-nameInstance.png)

- In **Quick Start** tab, choose **Amazon Linux**. Then choose **Amazon Linux 2023 AMI** and **Architecture** like below.
![EC2](/images/2.prerequisite/04-ami.png)

- Under the **Instance Type**, select **t2.micro**.
![EC2](/images/2.prerequisite/05-instanceType.png)

- **Key pair**, **Network settings**, **Configure storage** and **Advanced details** section set like default.
- Click **Launch instance**
![EC2](/images/2.prerequisite/06-launchInstance.png)

3. Back in the [**Instances**](https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Instances:) page, you'll see an EC2 instance that you just created. Wait for **Status check** is 2/2, f5 as needed.
![EC2](/images/2.prerequisite/07-ec2Instance.png)
