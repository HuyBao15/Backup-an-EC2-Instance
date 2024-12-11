---
title : "Restore an Amazon EC2 instance using AWS Backup"
date : "2024-12-05"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. In the [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), select **Vaults** in the left navigation pane under **My account**, then click the **Default** vault in the **Vaults** page.
![EC2](/images/4.restore/01-vaultDefault.png)

- Select the latest completed backup.
![EC2](/images/4.restore/02-latestBackup.png)

- Choose **Restore**
![EC2](/images/4.restore/03-restoreButton.png)

- In the Network settings pane, accept the defaults or specify the options for the **Instance type**, **Virtual Private Cloud (VPC)**, **Subnet**, **Security groups**, and **Instance IAM role settings**.

- Choose **Proceed with no IAM role** under the **Instance IAM role** section.
![EC2](/images/4.restore/04-defaults.png)

{{% notice info %}}
You must have two managed policies: AWSBackupServiceRolePolicyForBackup and AWSBackupServiceRolePolicyForRestores to continue the following step 
{{% /notice %}}

- Under the **Restore section** section, choose **Default role**
- Ignore **Advanced settings** (accept the defaults) and click **Restore backup** button.
![EC2](/images/4.restore/05-restoreBackup.png)

2. Check for your restored backup job under **Restore jobs** in the the [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/jobs/restore).
![EC2](/images/4.restore/06-restoreJobID.png)

3. Navigate to the [**Amazon EC2 console**](https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:) and select **Instances** in the left navigation pane to see the restored EC2 instance.
![EC2](/images/4.restore/07-instanceRestore.png)

