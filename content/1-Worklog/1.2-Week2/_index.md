---
title: "Worklog Week 2"
date: 2024-01-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Goals for Week 2:

* Learn about access management and system security using AWS IAM.
* Learn about Infrastructure as Code (IaC), get familiar with infrastructure tools (AWS CloudFormation, Terraform), and practice automated resource deployment.
* Learn the operating mechanisms of serverless with AWS Lambda and basic integrations.

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 15/06/2026 | **Learn about AWS IAM & Security:**<br>&emsp;+ Concepts of IAM User, Group, Role, and Policy.<br>&emsp;+ Classification of IAM Roles (Service Role, Cross-Account Role,...).<br>&emsp;+ Apply the Principle of Least Privilege. | <https://cloudjourney.awsstudygroup.com/><br><https://docs.aws.amazon.com/IAM/latest/UserGuide/> |
| Tue | 16/06/2026 | **Intern at company**<br>**Learn Infrastructure as Code (IaC):**<br>&emsp;+ Learn overview of AWS CloudFormation and AWS CDK.<br>&emsp;+ **Hands-on practice:** Structure a simple IaC template to initialize basic resources (VPC, Subnet, EC2 Instance). | <https://docs.aws.amazon.com/cloudformation/><br><https://docs.aws.amazon.com/cdk/v2/developerguide/> |
| Wed | 17/06/2026 | **Research Serverless AWS Lambda Service:**<br>&emsp;+ Concepts, architecture, and Lambda Function setup.<br>&emsp;+ Learn about Event Sources, Triggers, and Execution Role.<br>&emsp;+ **Hands-on practice:** Create a simple Lambda Function connected to an IAM Role and test via Function URL / API Gateway. | <https://cloudjourney.awsstudygroup.com/><br><https://docs.aws.amazon.com/lambda/> |
| Thu | 18/06/2026 | **Integration & Combined Practice:**<br>&emsp;+ Combine IAM Role + Lambda + CloudFormation to automate a small workflow deployment.<br>&emsp;+ Test assigning IAM Roles to EC2 servers and Lambda Functions. | <https://cloudjourney.awsstudygroup.com/> |
| Fri | 19/06/2026 | **Review & Weekly Wrap-up:**<br>&emsp;+ Review and optimize written CloudFormation templates.<br>&emsp;+ Debug IAM Policy authorization issues.<br>&emsp;+ Update Week 2 Worklog report documentation. | <https://cloudjourney.awsstudygroup.com/> |

### Results achieved in Week 2:

* **Security Administration & Authorization (IAM):**
  * Clear understanding of IAM operational mechanics: User, Group, Role, and Policy.
  * Differentiated Role types (especially Service Role for EC2 and Lambda) and applied the Principle of Least Privilege.
  * Deployed and tested IAM Roles to ensure safe service authorization.

* **Infrastructure as Code (IaC):**
  * Mastered infrastructure automation using IaC and clear template structures.
  * Successfully built simple CloudFormation/CDK templates to automatically initialize VPC, Subnet, and EC2 without manual Console operations.
  * Tested templates and managed resources via source code, increasing consistency in deployments.

* **Serverless Computing (AWS Lambda):**
  * Gained a solid grasp of how AWS Lambda operates, its lifecycle, and trigger mechanisms (Triggers/Event Sources).
  * Created and successfully deployed a simple Lambda Function with appropriate IAM Role for communicating with other AWS services.
  * Tested functionality using Lambda Function URL and evaluated integration with IAM policies.
