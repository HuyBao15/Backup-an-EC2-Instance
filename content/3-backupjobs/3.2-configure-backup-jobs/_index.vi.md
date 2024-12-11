---
title : "Cấu hình các tác vụ sao lưu AWS tự động"
date : "2024-12-05"
weight : 2
chapter : false
pre : " <b> 3.2. </b> "
---

1. Trong [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), chọn **Backup plans** ở thanh điều hướng bên trái dưới mục **My account**, sau đó nhấn Create backup plan.
![EC2](/images/3.awsbackup/10-backupPlans.png)

- Trên trang **Create backup plans** , chọn các tùy chọn sau:
  + Chọn **Build a new plan**. 
  + Nhập Tên kế hoạch sao lưu **backup plan name**.
  + Nhập Tên quy tắc sao lưu **Backup rule name**.
  + Chọn **Default** cho **Backup vault**. Hoặc tùy chọn, bạn có thể tạo vault sao lưu của riêng mình.
  + Chọn **Daily** cho **Backup frequency** (Tần suất sao lưu).
  + **Backup windows** bao gồm thời gian bắt đầu của cửa sổ sao lưu và thời lượng của cửa sổ (tính bằng giờ). Lab này sẽ đặt giá trị mặc định, hoặc bạn có thể tự cấu hình theo ý muốn.
  + Chọn **Forever** cho **Total retention period**.
  + Cuối cùng, nhấp vào **Create plan**.

![EC2](/images/3.awsbackup/11-createBackupPlan_part1.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part2.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part3.png)
![EC2](/images/3.awsbackup/11-createBackupPlan_part4.png)

2. Quay lại trang **Backup plans**, bạn sẽ thấy kế hoạch sao lưu mà bạn vừa tạo.
![EC2](/images/3.awsbackup/12-aBackupPlan.png) 

- Nhấp vào **Backup plan** để xem chi tiết. Trên trang **EC2-backup-plan**, chọn nút **Assign resources**.
![EC2](/images/3.awsbackup/13-assignResources.png)

- Nhập **Resource assignment name**(Tên phân công tài nguyên). Sau đó chọn **Default role** trong phần **IAM role**.
![EC2](/images/3.awsbackup/14-assignResources_part1.png)

- Trong phần **Define resource selection**, chọn **Include specific resource types**. Sau đó chọn **Resource types** là **EC2**. Cuối cùng, nhấn nút **Assign resources** .
![EC2](/images/3.awsbackup/14-assignResources_part2.png)

3. Trở lại trang [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/). Các công việc sao lưu sẽ xuất hiện trong mục **Jobs**.
![EC2](/images/3.awsbackup/15-jobsAppear.png)



