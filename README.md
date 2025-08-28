# Study DevLab – AWS-Powered EdTech Learning Platform

An **innovative web-based EdTech platform** designed to make learning web development interactive, scalable, and engaging.  
Study DevLab integrates **hands-on coding challenges, forums, real-time feedback, and personalized recommendations**, while leveraging **AWS cloud services** for scalability, monitoring, and cost efficiency.

---

## 🚀 Features

- **Interactive Learning Dashboard** – Hands-on coding in HTML, CSS, JS, React with real-time feedback.
- **Personalized Resource Recommendations** – Tailored videos, exercises, and tutorials based on performance.
- **Dynamic Challenge Evaluation** – Automated evaluation using Puppeteer + serverless workflows.
- **Community Forum** – Q&A, discussions, and collaborative learning.
- **Secure Authentication** – Role-based login with JWT, DynamoDB, and IAM.
- **Progress Tracking** – Leaderboards, scores, and detailed analytics dashboards.
- **Admin Panel** – Manage tutorials, challenges, and monitor platform usage.
- **Scalable Deployment** – Elastic Beanstalk, S3, CloudFront for availability.
- **Cost Monitoring** – CloudWatch, CloudTrail, and AWS Budgets for optimization.
- **Adaptive Learning** – Personalized learning paths and recommendations.

---

## 🏗️ Architecture

```mermaid
flowchart TD
  A[Frontend - React + Vite] -->|API Calls| B[Backend - Node.js/Express]
  B --> C[(DynamoDB)]
  B --> D[(S3 - Resource Storage)]
  A -->|Recommendations| E[Flask Service - Elastic Beanstalk]

  subgraph AWS_Cloud
    B
    C
    D
    E
  end

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
