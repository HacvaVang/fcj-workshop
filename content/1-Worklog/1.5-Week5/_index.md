---
title: "Worklog Week 5"
date: 2024-01-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Goals for Week 5:

* Automate project infrastructure setup and management using AWS CloudFormation.
* Write and standardize CloudFormation template files for all system resources.
* Test infrastructure deployment and updates via CloudFormation Stack.

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 06/07/2026 | **Build Network & Base Infrastructure (IaC):**<br>&emsp;+ Write CloudFormation template creating VPC, Public/Private Subnets, Internet Gateway, Route Tables.<br>&emsp;+ Practice deploying and testing basic network Stack. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| Tue | 07/07/2026 | **Build Compute & Scaling Layer (Compute & Scaling):**<br>&emsp;+ Write template initializing Security Groups, Launch Template, Auto Scaling Group, and Application Load Balancer (ALB).<br>&emsp;+ Integrate parameters (Parameters) and references (Ref/GetAtt) in CloudFormation. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| Wed | 08/07/2026 | **Build Storage & Database Layer (Storage & Database):**<br>&emsp;+ Write template initializing S3 Bucket, DynamoDB Table, and integrating KMS keys created last week.<br>&emsp;+ Package into Nested Stacks or Modular Templates. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| Thu | 09/07/2026 | **Deploy & Debug Master Stack:**<br>&emsp;+ Deploy entire project infrastructure via master CloudFormation Stack.<br>&emsp;+ Resolve errors arising during initialization (Rollback, Dependency errors). | <https://cloudjourney.awsstudygroup.com/> |
| Fri | 10/07/2026 | **Automate Updates & Weekly Wrap-up:**<br>&emsp;+ Practice using Change Sets to update infrastructure safely.<br>&emsp;+ Verify system availability post-deployment and update Week 5 report. | <https://cloudjourney.awsstudygroup.com/> |

### Results achieved in Week 5:

* **Infrastructure Automation (AWS CloudFormation):**
  * Digitized entire project infrastructure into source code (Code) in YAML/JSON format adhering to IaC standards.
  * Successfully wrote a complete CloudFormation template suite covering VPC, Subnet, ALB, ASG, EC2, S3, DynamoDB, and KMS.
  * Well-structured template design, easy to reuse and expand for subsequent phases.

* **Deployment Management (Stack Management):**
  * Successfully deployed the entire system through a single CloudFormation Stack creation step.
  * Practiced debugging Stack deployment errors, handling rollbacks and dependency errors.
  * Utilized Change Sets for safe infrastructure updates, minimizing service disruptions.
