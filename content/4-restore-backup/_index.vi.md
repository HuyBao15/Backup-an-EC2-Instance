---
title : "Khôi phục phiên bản Amazon EC2 bằng AWS Backup"
date : "2024-12-05"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

1. Trong [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), chọn **Vaults** trong thanh điều hướng bên trái dưới phần **My account**, sau đó chọn **Default** trên trang **Vaults**.
![EC2](/images/4.restore/01-vaultDefault.png)

- Chọn bản sao lưu mới nhất đã hoàn tất.
![EC2](/images/4.restore/02-latestBackup.png)

- Chọn **Restore**
![EC2](/images/4.restore/03-restoreButton.png)

- Trong phần Network settings, giữ nguyên cài đặt mặc định hoặc chỉ định các tùy chọn cho: **Instance type**, **Virtual Private Cloud (VPC)**, **Subnet**, **Security groups**, and **Instance IAM role settings**.

- Chọn **Proceed with no IAM role** trong phần **Instance IAM role**.
![EC2](/images/4.restore/04-defaults.png)

{{% notice info %}}
Để tiếp tục bước sau, bạn cần hai chính sách được quản lý: AWSBackupServiceRolePolicyForBackup và AWSBackupServiceRolePolicyForRestores để tiếp tục các bước sau.
{{% /notice %}}

- Trong phần **Restore section**, chọn **Default role**
- Bỏ qua phần **Advanced settings** (giữ nguyên mặc định) và nhấn nút **Restore backup**.
![EC2](/images/4.restore/05-restoreBackup.png)

2. Kiểm tra công việc khôi phục của bạn trong phần **Restore jobs** tại [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/jobs/restore).
![EC2](/images/4.restore/06-restoreJobID.png)

3. Chuyển đến [**Amazon EC2 console**](https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:) và chọn **Instances** trong thanh điều hướng bên trái để xem phiên bản EC2 đã được khôi phục.
![EC2](/images/4.restore/07-instanceRestore.png)

