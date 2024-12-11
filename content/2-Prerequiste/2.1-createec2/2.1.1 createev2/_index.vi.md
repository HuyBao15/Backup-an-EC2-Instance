---
title : "Create EC2"
date : "2024-12-05"
weight : 1
chapter : false
pre : " <b> 2.1.1 </b> "
---


#### Create EC2 
1. Truy cập [AWS Management Console](https://aws.amazon.com/console/) và mở **AWS EC2 Console**
   + Click **EC2**
![EC2](/images/2.prerequisite/01-openec2.png)


2. Trong bảng điều hướng bên trái của **AWS EC2 console**, dưới mục **Intances**, chọn **Intances**, sau đó chọn **Launch Instance**.
![EC2](/images/2.prerequisite/02-openinstances.png)

- Trên trang **Launch an instance**, tại mục **Name**, nhập tên cho instance.
![EC2](/images/2.prerequisite/03-nameInstance.png)

- Trông tab **Quick Start**, chọn **Amazon Linux**. Sau đó chọn **Amazon Linux 2023 AMI** và **Architecture** như hình bên dưới.
![EC2](/images/2.prerequisite/04-ami.png)

- Dưới mục **Instance Type**, chọn **t2.micro**.
![EC2](/images/2.prerequisite/05-instanceType.png)

- Ở các mục **Key pair**, **Network settings**, **Configure storage** và **Advanced details** để mặc định.
- Nhấp vào **Launch instance**
![EC2](/images/2.prerequisite/06-launchInstance.png)

3. Trở lại trang [**Instances**](https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Instances:), bạn sẽ thấy một phiên bản EC2 vừa được tạo. Chờ cho **Status check**  2/2, và làm mới trang(F5) nếu cần.
![EC2](/images/2.prerequisite/07-ec2Instance.png)
