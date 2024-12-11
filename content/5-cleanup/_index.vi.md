---
title : "Dọn dẹp tài nguyên"
date :  "2024-12-05" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

Chúng ta sẽ thực hiện các bước sau để xóa tài nguyên đã tạo trong bài thực hành này.

#### Xóa phiên bản EC2

1. Truy cập [EC2 service management console](https://console.aws.amazon.com/ec2/v2/home)
   + Nhấp vào **Instances**.
   + Chọn cả **EC2 Backup Lab** và các phiên bản  **EC2 Backup Lab** đã được khôi phục.
   + Nhấn vào **Instance state**.
   + Nhấn vào **Terminate instance**, sau đó nhấn vào **Terminate** để xác nhận.
![EC2](/images/5.cleanup/01-deleteRecoveryPoint.png)

#### Xóa điểm khôi phục của AWS Backup
1.  Truy cập [AWS Backup Console](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)
   + Nhấn vào **Vaults**.
   + Nhấn vào kho lưu trữ **Default**.
   + Chọn **Recovery point**.
   + Nhấn vào **Actions**, sao đó chọn **delete**.
![EC2](/images/5.cleanup/01-deleteRecoveryPoint.png)

#### Xóa kế hoạch sao lưu AWS Backup
1. Truy cập [AWS Backup Console](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)
   + Chọn **Backup plans**.
   + Nhấp vào tên kế hoạch sao lưu **EC2-backup-plan** .
   + Chọn **EC2-resources** trong phần **Resource assignments**.
   + Nhấn **Delete**.
![EC2](/images/5.cleanup/02-deleteBackupPlans.png)




