---
title : "Giới thiệu"
date : 2024-01-01 
weight : 1
chapter : false
pre : " <b> 5.1. </b> "
---

#### Giới thiệu về AWS Lamdba

#### Giới thiệu về AWS Gateway API

#### Giới thiệu về AWS DynamoDB

#### Giới thiệu về AWS S3

#### Giới thiệu về AWS CloudFormation

#### Giới thiệu về AWS CDK


#### Tổng quan về workshop
Trong workshop này, bạn sẽ sử dụng hai VPC.
+ **"VPC Cloud"** dành cho các tài nguyên cloud như Gateway endpoint và EC2 instance để kiểm tra.
+ **"VPC On-Prem"** mô phỏng môi trường truyền thống như nhà máy hoặc trung tâm dữ liệu của công ty. Một EC2 Instance chạy phần mềm StrongSwan VPN đã được triển khai trong "VPC On-prem" và được cấu hình tự động để thiết lập đường hầm VPN Site-to-Site với AWS Transit Gateway. VPN này mô phỏng kết nối từ một vị trí tại TTDL (on-prem) với AWS cloud. Để giảm thiểu chi phí, chỉ một phiên bản VPN được cung cấp để hỗ trợ workshop này. Khi lập kế hoạch kết nối VPN cho production workloads của bạn, AWS khuyên bạn nên sử dụng nhiều thiết bị VPN để có tính sẵn sàng cao.

<img src="{{ 'images/5-Workshop/5.1-Workshop-overview/diagram1.png' | relURL }}" alt="overview">