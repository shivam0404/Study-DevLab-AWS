# 📘 Study DevLab – AWS-Powered EdTech Platform  

> An **interactive, cloud-native EdTech platform** that combines web development practice, automated evaluation, AI-driven recommendations, and community learning — built entirely on **AWS Cloud Services** for scalability, cost-efficiency, and reliability.  

---

## ✨ Key Highlights  

- ☁️ **AWS-First Approach** – Deployed with **Elastic Beanstalk, S3, DynamoDB, CloudFront, CloudWatch, CloudTrail, IAM, and AWS Budgets**.  
- 🎯 **Interactive Web Development Learning** – Hands-on coding with real-time validation and feedback.  
- 🤖 **AI-Powered Recommendations** – Flask microservice suggests tailored resources & tutorials.  
- 📊 **Monitoring & Cost Control** – CloudWatch (metrics), CloudTrail (audits), AWS Budgets (alerts).  
- 👥 **Community-Centric** – Forums, Q&A, and leaderboards for collaborative learning.  
- 🛠️ **Admin Tools** – Full management of tutorials, challenges, and platform usage.  

---

## 🚀 Features  

- **Interactive Learning Dashboard** – Real-time coding practice with React, HTML, CSS, and JS.  
- **Personalized Resource Recommendations** – AI-driven Flask engine for dynamic learning paths.  
- **Automated Challenge Evaluation** – Puppeteer-based validation of coding challenges.  
- **Community Forum** – Engage with peers, ask questions, and share insights.  
- **Secure Authentication** – Role-based access using JWT, DynamoDB, and AWS IAM.  
- **Progress Tracking** – Leaderboards, scores, and analytics dashboards.  
- **Scalable Deployment** –  
  - Backend → AWS Elastic Beanstalk  
  - Frontend → AWS Amplify / S3 + CloudFront  
  - File Storage → S3  
- **Cost & Performance Monitoring** – CloudWatch, CloudTrail, and AWS Budgets.  

---

## 🏗️ System Architecture  

```mermaid
flowchart TD
  A[Frontend - React + Vite] -->|API Calls| B[Backend - Node.js/Express]
  B --> C[(DynamoDB - Users, Posts, Forum Data)]
  B --> D[(S3 - Content & Learning Materials)]
  A -->|Recommendations| E[Flask Recommender Service]

  subgraph AWS_Cloud
    B
    C
    D
    E
  end

⚡ Tech Stack & AWS Services

Frontend: React, Vite, TailwindCSS, Cypress

Backend: Node.js, Express, Puppeteer

Microservices: Flask (Recommendation Engine)

AWS Services:

Elastic Beanstalk – Backend & Flask deployment

Amplify / S3 + CloudFront – Frontend hosting

DynamoDB – Scalable NoSQL database

S3 – File & resource storage

CloudWatch – Monitoring CPU, latency, errors

CloudTrail – API activity logging

AWS Budgets – Cost optimization & alerts

IAM – Secure access control

📂 Project Structure
Study-DevLab-AWS/
├─ backend/                 # Node/Express API
│  ├─ src/controllers/
│  ├─ server.cjs / app.cjs
│  ├─ package.json
│  ├─ .env.example
│  └─ Dockerfile
├─ frontend/                # React + Vite app
│  ├─ src/ ├─ public/
│  ├─ package.json
│  └─ vite.config.js
├─ cypress/                 # End-to-end tests
├─ .github/workflows/       # CI/CD pipelines
├─ .gitignore
├─ LICENSE
├─ README.md
└─ docs/                    # Architecture diagrams, screenshots, ADRs

🛠️ Setup Instructions
1. Clone the Repo
git clone https://github.com/vishal-n2403/Study-DevLab-AWS.git
cd Study-DevLab-AWS

2. Backend Setup
cd backend
cp .env.example .env   # Add AWS + JWT configs
npm install
npm run dev

3. Frontend Setup
cd frontend
npm install
npm run dev

4. Run Cypress Tests
cd cypress
npx cypress open

🔐 Environment Variables
Backend .env.example
PORT=5000
AWS_REGION=us-east-1
DDB_USERS_TABLE=userr-info
DDB_POSTS_TABLE=posts
S3_BUCKET_FOR_DATA=awsrecom
JWT_SECRET=change-me
RECOMMENDER_API_URL=http://<flask-eb-endpoint>

Frontend .env
VITE_API_BASE_URL=http://localhost:5000

📦 Deployment Workflow

Frontend → AWS Amplify or S3 + CloudFront

Backend → AWS Elastic Beanstalk (Node.js)

Recommender Service → AWS Elastic Beanstalk (Python)

Monitoring → AWS CloudWatch dashboards + alarms

Auditing → AWS CloudTrail logs

Cost Control → AWS Budgets alerts

📄 License

Distributed under the MIT License. See LICENSE
 for details.