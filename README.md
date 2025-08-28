# 🚀 DevLab – Innovative Code Evaluation and Learning Platform  

[![AWS](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazon-aws)](https://aws.amazon.com/)  
[![React](https://img.shields.io/badge/Frontend-React-blue?logo=react)](https://reactjs.org/)  
[![Node.js](https://img.shields.io/badge/Backend-Node.js-green?logo=node.js)](https://nodejs.org/)  
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)  

An **Ed-Tech Web Development Learning Platform** designed to provide interactive coding challenges, real-time feedback, adaptive resource recommendations, and community collaboration – all powered by **AWS Cloud**.  

---

## 📖 About  
DevLab enables learners to practice **HTML, CSS, JavaScript, React, and Tailwind** coding challenges in a secure and scalable environment. It integrates **AWS services** for deployment, monitoring, and authentication while ensuring an engaging user experience.  

---

## 🎯 Objectives  
- Provide an **interactive coding environment** with real-time evaluation.  
- Deliver **personalized learning paths** with ML-driven recommendations.  
- Enable **secure authentication & role-based access**.  
- Ensure **scalable architecture** with AWS Elastic Beanstalk & CloudFront.  
- Foster **community-driven learning** via forums and discussions.  
- Track learner progress through **analytics dashboards**.  

---

## 🔑 Features  
- 👤 **User Authentication & Profiles** – Secure login, registration, role-based access.  
- 🖥 **Interactive Coding Dashboard** – Real-time code editor & feedback.  
- 🏆 **Challenges & Progress Tracking** – Leaderboards, scoring system.  
- 🎯 **Resource Recommendation System** – Personalized tutorials & exercises.  
- 💬 **Discussion Forum** – Collaborative Q&A and topic-based discussions.  
- 📊 **Performance Analytics** – Visual dashboards with detailed reports.  
- ⚡ **Serverless Evaluation** – AWS Lambda for real-time code validation.  
- 🔒 **Data Security & Compliance** – IAM, Cognito, and encryption standards.  

---

## 🏗️ Modules  
1. User Authentication & Profile Management  
2. Interactive Learning Dashboard  
3. Challenges & Progress Tracking  
4. Resource Recommendation System  
5. Discussion Forum  
6. Admin Panel for Content Management  
7. Real-Time Challenge Evaluation  
8. Frontend Search & Content Display  
9. Monitoring & Reporting  
10. Cost Monitoring & Optimization  

---

## 🛠️ Tech Stack  
**Frontend**: React, Tailwind CSS, AWS Amplify  
**Backend**: Node.js, Express.js, Flask  
**Database**: DynamoDB  
**Deployment**: AWS Elastic Beanstalk, EC2, CloudFront, S3  
**Monitoring & Security**: AWS CloudWatch, CloudTrail, IAM, Cognito  

---

## ☁️ AWS Services Used  
- **Amazon EC2** – Compute resources for backend services.  
- **Amazon S3** – Static assets and user resource storage.  
- **AWS DynamoDB** – User data, progress tracking, forum content.  
- **AWS Amplify** – Frontend hosting and CI/CD pipeline.  
- **AWS Elastic Beanstalk** – Scalable backend deployment.  
- **AWS CloudWatch & CloudTrail** – Monitoring, logging, auditing.  
- **AWS IAM & Cognito** – Authentication, authorization, and access control.  

---

## 📐 Architecture  
```mermaid
flowchart TD
    A[Frontend - React/Tailwind] -->|API Calls| B[AWS API Gateway]
    B --> C[Backend - Node.js/Flask]
    C --> D[DynamoDB - User Data]
    C --> E[S3 - Resources]
    C --> F[Lambda - Code Evaluation]
    B --> G[Amplify/CloudFront - Hosting]
    G --> A
    C --> H[CloudWatch & CloudTrail - Monitoring]

## 📸 Screenshots

### 🔑 Login / Registration
![Login Screenshot](assets/screenshots/login.png)
