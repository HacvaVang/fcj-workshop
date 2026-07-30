---
title: "Worklog Week 7"
date: 2024-02-12
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Goals for Week 7:

* Conduct integrated testing of the entire application and infrastructure for the team project.
* Draft and complete hands-on lab documentation (Workshop Documentation).
* Learn theory and practice standalone AWS WAF (Web Application Firewall) configuration.

### Tasks to implement this week:
| Day | Date | Tasks | Reference Materials |
| --- | ---- | ----- | ------------------- |
| Mon | 20/07/2026 | **Project Integration Testing:**<br>&emsp;+ Test end-to-end flow between Frontend, Backend, DynamoDB, and S3.<br>&emsp;+ Review and debug project API / Database connections. |  |
| Tue | 21/07/2026 | **Learn AWS WAF Theory:**<br>&emsp;+ Concepts of Web ACL, Rules, Rule Groups.<br>&emsp;+ Common web attack mitigation mechanisms: SQL Injection (SQLi), Cross-Site Scripting (XSS), Rate-based (DDoS). | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| Wed | 22/07/2026 | **Hands-on AWS WAF:**<br>&emsp;+ Create test Web ACL and add AWS Managed Rule Groups.<br>&emsp;+ **Hands-on practice:** Create separate test environment to attach Web ACL and test traffic blocking/allowing capability. | <https://docs.aws.amazon.com/waf/latest/developerguide/> |
| Thu | 23/07/2026 | **Build Workshop Documentation:**<br>&emsp;+ Draft step-by-step lab guide for project practical workshop.<br>&emsp;+ Take screenshots and annotate key technical notes. |  |
| Fri | 24/07/2026 | Check Workshop documentation completion progress and summarize Week 7 report. |  |

### Results achieved in Week 7:

* **System Integration Testing:**
  * Executed end-to-end flow tests across Frontend, Backend, DynamoDB, and S3.
  * Reviewed and debugged API connections, authentication mechanisms, and data pipelines.

* **Learn & Practice AWS WAF:**
  * Thoroughly understood Web ACL, Rule Groups, and AWS WAF Layer 7 traffic filtering mechanisms.
  * Practiced creating Web ACLs and adding AWS Managed Rule Groups targeting SQLi, XSS, and rate-limiting.
  * Tested request blocking/allowing functionality and evaluated application protection efficacy.

* **Build Workshop Documentation:**
  * Drafted comprehensive, step-by-step practical guides complete with annotated diagrams and technical notes.
  * Finalized Workshop document draft enabling external users to reproduce the project from scratch.
