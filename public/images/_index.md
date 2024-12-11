---
title : "Clean up resources"
date :  "2024-12-05" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

We will take the following steps to delete the resources we created in this exercise.

#### Delete EC2 Instances

1. Go to [EC2 service management console](https://console.aws.amazon.com/ec2/v2/home)
   + Click **Instances**.
   + Select both **EC2 Backup Lab** and restored **EC2 Backup Lab** instances.
   + Click **Instance state**.
   + Click **Terminate instance**, then click **Terminate** to confirm.

#### Delete the AWS Backup recovery point
1.  Go to [AWS Backup Console](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)
   + Click **Vaults**.
   + Click **Default** vault.
   + Choose the **Recovery point**.
   + Click **Actions**, then click **delete**.
![EC2](/images/5.cleanup/01-deleteRecoveryPoint.png)

#### Delete the AWS Bacup Plans
1. Go to [AWS Backup Console](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)
   + Click **Backup plans**.
   + Click the **EC2-backup-plan** Backup plan name.
   + Choose **EC2-resources** under the **Resource assignments** section.
   + Click **Delete**.
![EC2](/images/5.cleanup/02-deleteBackupPlans.png)




