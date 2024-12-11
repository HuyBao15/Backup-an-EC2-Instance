---
title : "Tạo tác vụ AWS Backup theo yêu cầu của phiên bản Amazon EC2"
date : "2024-12-05"
weight : 1
chapter : false
pre : " <b> 3.1. </b> "
---

1. Mở [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/)

2. Cấu hình các dịch vụ được sử dụng với AWS Backup

- Ở phía bên trái của [**AWS Backup console**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), trong **My account**, chọn Cài đặt.
![EC2](/images/3.awsbackup/02-settings.png)

- Trên trang **Service opt-in**, chọn **Configure resources**.
![EC2](/images/3.awsbackup/03-configureResources.png)

- Trên trang **Configure resources**, sử dụng các công tắc chuyển đổi để bật hoặc tắt các dịch vụ được sử dụng với AWS Backup. Trong phòng thí nghiệm này, chỉ chọn EC2, sau đó nhấp vào **Confirm**.
![EC2](/images/3.awsbackup/04-selectEC2.png)

1. Quay trở lại [**AWS Backup**](https://ap-southeast-2.console.aws.amazon.com/backup/home?region=ap-southeast-2#/), trong **My account** ở ngăn điều hướng bên trái, chọn  **Protected resources**.
![EC2](/images/3.awsbackup/05-protectedResources.png)

- Nhấp vào nút **Create on-demand backup**.
![EC2](/images/3.awsbackup/06-createOnDemand.png)

- Trên trang Tạo bản sao lưu theo yêu cầu, hãy chọn các tùy chọn sau:
  + Chọn **Resource type** là EC2.
  + Chọn Instance ID of the EC2 rmà bạn vừa tạo ở chương trước.
  + Chọn **Create backup now** trong **Backup window**.
  + Chọn **Forever** cho **TOtal retention period**.
  + Select **Default** cho **Backup vault**. Tùy chọn, bạn có thể tạo kho lưu trữ sao lưu của riêng mình.
  + Chọn **Default role** trong **IAM role**.
  + Nhấp chọn **Create on-demand backup**. 
![EC2](/images/3.awsbackup/07-createOnDemand_part1.png)
![EC2](/images/3.awsbackup/08-createOnDemand_part2.png)

- Trên trang **Jobs**, bạn sẽ thấy các công việc sao lưu mà bạn đã tạo.
![EC2](/images/3.awsbackup/09-aBackupjob.png)

- Chọn **Backup job ID** để xem thông tin chi tiết về tác vụ đó.





