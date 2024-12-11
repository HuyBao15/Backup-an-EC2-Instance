---
title : "Configure automatic AWS Backup jobs"
date : "2024-12-05"
weight : 2
chapter : false
pre : " <b> 3.2. </b> "
---

1. In the [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), select **Backup plans** in the left navigation pane under **My account**, and then Create backup plan.
![EC2](/images/3.awsbackup/10-backupPlans.png)

- Under the **Create backup plans** page, choose the following options:
  + select **Build a new plan**. 
  + Enter **backup plan name**.
  + Enter **Backup rule name**.
  + Select **Default** for **Backup vault**. Optionally, you can create your own backup vault.
  + Select **Daily** for **Backup frequency**.
  + **Backup windows** consist of the time that the backup window begins and the duration of the window in hours. This lab will set default or you can set whatever you want.
  + Select **Forever** for **Total retention period**.
  + Finally, click **Create plan**.

![EC2](/images/3.awsbackup/11-createBackupPlan_part1.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part2.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part3.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part4.png)

2. Back in to the **Backup plans** page, you will see the backup plan you just created.
![EC2](/images/3.awsbackup/12-aBackupPlan.png) 

- Click that **Backup plan** to see details. Then on the **EC2-backup-plan** page, choose **Assign resources** button.
![EC2](/images/3.awsbackup/13-assignResources.png)

- Enter **Resource assignment name**. Then choose **Default role** under **IAM role** section.
![EC2](/images/3.awsbackup/14-assignResources_part1.png)

- Under **Define resource selection**, choose **Include specific resource types**. Then select **Resource types** is **EC2**. Finally, click **Assign resources** button.
![EC2](/images/3.awsbackup/14-assignResources_part2.png)

3. Navigate to the [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/). The backup jobs will be seen under **Jobs**.
![EC2](/images/3.awsbackup/15-jobsAppear.png)



