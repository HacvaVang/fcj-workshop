---
title: "Worklog Week 6"
date: 2024-02-05
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Goals for Week 6:

* Report project infrastructure deployment progress to Mentor and incorporate feedback.
* Modify, optimize, and add necessary services into the CloudFormation template.
* Research and integrate Amazon CloudFront Content Delivery Network (CDN) to optimize performance.

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 13/07/2026 | **Intern at company**<br>**Team Progress Report:**<br>&emsp;+ Report infrastructure and application deployment progress to Mentor/Internship Unit.<br>&emsp;+ Record architecture feedback and additional optimization requirements. | <https://cloudjourney.awsstudygroup.com/> |
| Tue | 14/07/2026 | **Modify & Refactor Infrastructure:**<br>&emsp;+ Update CloudFormation template based on feedback (optimize Security Groups, fine-tune Auto Scaling parameters).<br>&emsp;+ Update Change Set and re-test infrastructure. | <https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/> |
| Wed | 15/07/2026 | **Learn Amazon CloudFront (CDN):**<br>&emsp;+ Concepts of CDN, Edge Locations, Origin, Caching Policy.<br>&emsp;+ Origin Access Control (OAC) security mechanism when combining CloudFront with S3. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| Thu | 16/07/2026 | **Hands-on Amazon CloudFront Configuration:**<br>&emsp;+ Create CloudFront Distribution combining S3 Bucket (for static files) and ALB (for dynamic content).<br>&emsp;+ Configure Origin Access Control (OAC) to block direct access to S3 Bucket. | <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/> |
| Fri | 17/07/2026 | **Performance Testing & Wrap-up:**<br>&emsp;+ Test page load speed before and after passing through CloudFront (Latency / Bandwidth optimization).<br>&emsp;+ Add CloudFront resources to CloudFormation template and finalize Week 6 report. | <https://cloudjourney.awsstudygroup.com/> |

### Results achieved in Week 6:

* **Project Infrastructure Optimization:**
  * Successfully refactored CloudFormation template, removed redundant configurations, standardized parameters, and enhanced scalability.
  * Updated Security Groups to only open required ports, fine-tuned access policies between ALB and EC2, reducing attack surface and improving security.
  * Adjusted Auto Scaling Group parameters (min/max instances, scaling policy) to balance cost and performance in the internship environment.
  * Added CloudFront to template and created Change Sets to test infrastructure updates safely.

* **Content Delivery (Amazon CloudFront):**
  * Gained thorough understanding of CDN principles, caching, origin modes, Edge Locations, and AWS content delivery networks.
  * Successfully deployed CloudFront Distribution for both static files on S3 and dynamic services via ALB.
  * Configured Origin Access Control (OAC) with S3 Origin, ensuring S3 access only via CloudFront, strengthening static data security.
  * Defined suitable cache policies for static content, reducing direct load on S3 and accelerating page loads globally.
  * Tested performance before and after CloudFront usage, verifying latency reduction, faster browsing speed, and optimized static content bandwidth.
