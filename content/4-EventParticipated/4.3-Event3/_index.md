---
title: "Event 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Summary Report "FCAJ x Agentic AI Build Week"

### Event Purpose
- Share best practices in modern application design and integrating Agentic AI into operational workflows.
- Share company culture, innovative mindsets, and practical experiences from leading enterprises/experts (such as AWS).
- Create a technical practice playground, promoting innovation and solving real-world business challenges using AI technology.

---

### List of Speakers
- **Mr. Nguyen Gia Hung**: Head of Solution Architecture, AWS Vietnam.
- **Mr. Joseph Marazota**: Head of Technology, AWS ASEAN.
- **One Team**: Winner of AABW Hackathon.
- **Signal Scout**: Runner-up of AABW Hackathon.
- **Plan V**: Participant team in AABW Hackathon.
- **3KA**: Participant team in AABW Hackathon.
- **Six Pillar Team**: Participant team in AABW Hackathon.

---

### Highlighted Content

#### AI-Powered Conversation Ordering
- **Problem**: Current AI food ordering solutions are prone to errors when processing natural language, disappointing customers. Additionally, switching channels from chat to app download creates friction and loses engagement.
- **Solution**: Built a multi-channel conversational AI Agent on Zalo/WhatsApp, interacting naturally with clear order confirmations to prevent mistakes.
- **Architecture & Tech**: Utilized AI web scraping (Tiny Fish, Abify) to collect menus/promotions from KFC; modular architecture easily adapting business logic; AI Agent featuring session memory.
- **Cost & Performance**: Latency of 0.3 - 0.4s, infrastructure cost ~$88/month (~$0.006/order), saving 60% in infrastructure costs thanks to design optimization.

#### Solutional Architect Professional Native App
- **Problem**: Resolving pressure for Cloud Solution Architects (SAs) who need to rapidly design, price, and deploy infrastructure within a few hours.
- **Solution**: AI-native app automating architecture drafting, pricing, and Infrastructure as Code (Terraform, CloudFormation) generation via natural language or business documents.
- **Highlights**: Supports Blacklist validation filtering disallowed services, capable of stepwise reasoning explaining design rationale, and reusing IaC modules.

#### Build a production-ready AI application using AWS AI/ML
- **AWS Service Integration**: Leveraged solutions such as AWS Amplify, Cognito, Lambda, Fargate, S3, DynamoDB to ensure production readiness.
- **Multi-Agent System Application**: Combined crawler agents, noise filter agents, analysis/scoring agents, and human review (Human-in-the-loop).
- **Enterprise Strategy Analysis**: Rapidly scraped and analyzed competitor data from financial reports and websites, forecasting strategic impact at $35 - $130/month cost.

#### Smart Human-flow Evaluation, Prediction, Hazard Detection, Response and Dispatch (S.H.E.P.H.R.D)
- **Problem**: Managing crowd congestion at airports, events, and retail stores requires proactive control rather than manual monitoring.
- **Solution**: Real-time video analysis system combining Edge Computing and AWS Cloud.
- **Model & Architecture**: Utilized YOLO v2.6 Small model to detect and track individuals by area (zonal tracking); data streams fed into AWS Fargate, stored in DynamoDB/S3.
- **Features**: Calculated wait times, suggested control measures, dispatched automated alerts, and supported operator intervention (Operator Cockpit).

#### Adaptive AML Workflow Engine
- **Problem**: The financial sector faces massive volumes of suspicious transaction alerts, 90-95% of which are false positives. Manual procedures consume time and cost.
- **Solution**: AI engine optimizing Anti-Money Laundering (AML) investigation workflows, automatically aggregating data from multiple sources (transaction history, KYC, screening).
- **Impact**: Reduced processing time from days/hours down to minutes, providing auditable and explainable evidence logs without altering the human decision-making role.

#### Hackathon Participation Experience
- **Working under time pressure**: Challenges extending until 3-4 AM, requiring rapid problem-solving spirits.
- **Building MVP & Demo**: Emphasized focusing on core problems, realistic scope control, and preparing live-running demos rather than presenting pure theory.
- **Conflict Management & Communication**: Multilingual team with diverse skills needing active listening, clear role assignments, and unified goals to resolve disagreements.

---

### Key Takeaways
- **AI Product Design Mindset**: Need to focus 70%+ on solving real business use cases rather than showing off pure technology.
- **Multi-Agent & Human-in-the-loop Applications**: Flexibly combine specialized Agents while keeping human intervention for low confidence cases.
- **Cost & Performance Optimization**: System design techniques reducing up to 60% of AI operating costs, leveraging serverless architecture (Lambda, Fargate).
- **Soft Skills**: Lessons in teamwork under high pressure, project scope management, and Q&A presentation skills before judges.

---

### Application to Work
- **Business Process Automation**: Apply AI Agent models to automate data aggregation, document info extraction, and automated report generation.
- **System Design Optimization**: Utilize Cloud/AI architectural principles from AWS to build scalable and cost-effective solutions.
- **Enhance Customer Experience**: Explore integrating conversational AI with session memory into direct user interaction channels without forcing app switches.

---

### Event Experience

#### Learning from highly specialized speakers
- Received strategic vision sharing from Mr. Joseph Marazota and Mr. Nguyen Gia Hung on the transition from quarterly release cycles to minute-by-minute continuous delivery, along with AI's role in reshaping industries.

#### Practical technical experience
- Direct access to advanced technical solutions: YOLO v2.6 for real-time video processing, Multi-Agent workflows, AI scraping (Tiny Fish), automated IaC generation (Terraform/CloudFormation).

#### Applying modern tools
- Experienced integrating leading AWS services (Amplify, Cognito, Lambda, Fargate, DynamoDB, S3) with modern AI/ML models to build production-ready products.

#### Networking and exchange
- Expanded networking with top experts and speakers from AWS and energetic tech enthusiasts in the HCMC AI community.

#### Key Lessons Learned
- Always maintain continuous learning mindsets, embrace risks, and take on challenges at hackathons. No matter how good an idea is, focusing on an executable MVP that solves real user needs is the deciding factor for success.

#### Photos from participating in the event
![Event picture 1](/fcj-workshop/images/4-Events/event-3.1.jpg)
![Event picture 2](/fcj-workshop/images/4-Events/event-3.2.jpg)