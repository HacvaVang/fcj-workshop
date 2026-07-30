---
title: "Worklog Week 3"
date: 2024-01-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Goals for Week 3:

* Officially finalize group topic, complete overall architecture diagram, and detailed task assignment for team members.
* Research Auto Scaling and Load Balancing mechanisms for EC2 virtual servers.
* Learn object storage service Amazon S3 and NoSQL database management system Amazon DynamoDB.
* Practice integrating S3 and DynamoDB with compute services (EC2 / AWS Lambda).

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 22/06/2026 | **Team Meeting - Choose & Finalize Topic:**<br>&emsp;+ Discuss project ideas, analyze feasibility, and agree on official topic.<br>&emsp;+ Draft overall system architecture diagram on draw.io. | <https://cloudjourney.awsstudygroup.com/> |
| Tue | 23/06/2026 | **Scaling with AWS EC2:**<br>&emsp;+ Learn Auto Scaling Group (ASG) and Elastic Load Balancing (ALB/NLB) mechanisms.<br>&emsp;+ AMI (Amazon Machine Image) and Launch Template concepts.<br>&emsp;+ **Hands-on practice:** Create Launch Template, set up Auto Scaling Group combined with ALB to automatically adjust EC2 instance count based on load. | <https://docs.aws.amazon.com/autoscaling/ec2/userguide/> |
| Wed | 24/06/2026 | **Amazon S3 Storage Service:**<br>&emsp;+ Learn Bucket, Object, Storage Classes, and Lifecycle Policies concepts.<br>&emsp;+ S3 Security: S3 Bucket Policy, Block Public Access, and Access Control List (ACL).<br>&emsp;+ **Hands-on practice:** Create S3 Bucket, configure permissions, and store static files (Static Website Hosting / Media Assets). | <https://docs.aws.amazon.com/AmazonS3/latest/userguide/> |
| Thu | 25/06/2026 | **Amazon DynamoDB NoSQL Database:**<br>&emsp;+ Table, Partition Key, Sort Key, and Secondary Indexes (GSI/LSI) concepts.<br>&emsp;+ **Hands-on practice:** Initialize DynamoDB table, perform data operations (CRUD) via AWS Management Console and AWS CLI/SDK. | <https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/> |
| Fri | 26/06/2026 | **Integration & Weekly Wrap-up:**<br>&emsp;+ **Integration practice:** Write applications on EC2 / Lambda Functions to read/write data from DynamoDB and store files in S3.<br>&emsp;+ Test deployed services and compile Week 3 report. | <https://cloudjourney.awsstudygroup.com/> |

### Results achieved in Week 3:

* **Team Topic:**
  * Agreed on team internship project topic.
  * Drafted and completed overall system architecture diagram on *draw.io*, illustrating data flow between components.

* **Scaling & Load Balancing (EC2 Scaling):**
  * Mastered working principles of Elastic Load Balancer (ALB) and Auto Scaling Group (ASG).
  * Initialized Launch Template and deployed EC2 system capable of automatically scaling instance count up/down based on traffic.
  * Configured scaling policies to balance performance and cost.

* **Object Storage (Amazon S3):**
  * Understood data organization, S3 Bucket Policy security configurations, and Block Public Access.
  * Successfully deployed S3 Bucket to store static resources and ensured safe access control.

* **NoSQL Database (Amazon DynamoDB):**
  * Practiced designing DynamoDB tables with appropriate Partition Key, Sort Key, and secondary indexes.
  * Performed successful CRUD operations and connected EC2/Lambda applications to DynamoDB via AWS SDK.

* **Application Integration:**
  * Successfully connected compute services with S3 and DynamoDB.
  * Tested data read/write flow from backend to database and storage.
