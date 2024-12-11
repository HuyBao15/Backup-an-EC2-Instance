---
title : "Create an on-demand AWS Backup job of an Amazon EC2 instance"
date : "2024-12-05"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---

1. Open the [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)

2. Configure the services used with AWS Backup

- On the left side of [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), under **My account**, choose Settings.
![EC2](/images/3.awsbackup/02-settings.png)

- On the **Service opt-in** page, choose **Configure resources**.
![EC2](/images/3.awsbackup/03-configureResources.png)

- On the **Configure resources** page, use the toggle switches to enable or disable the services used with AWS Backup. In this lab, only select EC2, then click **Confirm**.
![EC2](/images/3.awsbackup/04-selectEC2.png)

3. Back in the [**AWS Backup**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/) console, under **My account** in the left navigation pane, select **Protected resources**.
![EC2](/images/3.awsbackup/05-protectedResources.png)

- Click **Create on-demand backup** button.
![EC2](/images/3.awsbackup/06-createOnDemand.png)

- On the Create on-demand backup page, choose the following options:
  + Select **Resource type** is EC2.
  + Select Instance ID of the EC2 resource that you just created in the previous chapter.
  + Choose **Create backup now** under the **Backup window**.
  + Select **Forever** for **TOtal retention period**.
  + Select **Default** for **Backup vault**. Optionally, you can create your own backup vault.
  + Choose **Default role** under **IAM role**.
  + Click **Create on-demand backup**.
![EC2](/images/3.awsbackup/07-createOnDemand_part1.png)
![EC2](/images/3.awsbackup/08-createOnDemand_part2.png)

- On the **Jobs** page, you will see the backup jobs you created.
![EC2](/images/3.awsbackup/09-aBackupjob.png)

- Choose the **Backup job ID** to see the details of that job.



