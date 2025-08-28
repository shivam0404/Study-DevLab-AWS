# 🚀 DevLab — Innovative Code Evaluation & Learning Platform

[![Cloud](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazon-aws)](https://aws.amazon.com/)
[![Frontend](https://img.shields.io/badge/Frontend-React-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![Styling](https://img.shields.io/badge/UI-TailwindCSS-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Backend](https://img.shields.io/badge/Backend-Node.js-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![Evaluator](https://img.shields.io/badge/Evaluator-Puppeteer-40B5A4?logo=google-chrome&logoColor=white)](https://pptr.dev/)
[![ML Reco](https://img.shields.io/badge/Service-Flask-000000?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Database](https://img.shields.io/badge/DB-DynamoDB-4053D6?logo=amazondynamodb&logoColor=white)](https://aws.amazon.com/dynamodb/)
[![Storage](https://img.shields.io/badge/Storage-S3-569A31?logo=amazon-s3&logoColor=white)](https://aws.amazon.com/s3/)
[![CI/CD](https://img.shields.io/badge/Deploy-Elastic%20Beanstalk-3B3B3B?logo=awselasticbeanstalk&logoColor=white)](https://aws.amazon.com/elasticbeanstalk/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

DevLab is an **AWS-powered Ed-Tech platform** for learning modern web development with **interactive coding challenges, real-time feedback, adaptive recommendations,** and a **community forum**. It combines a **React** front-end (with Monaco editor) and a **Node/Express** API with a **headless Chrome (Puppeteer) evaluator**, plus a **Flask** microservice for recommendations—**scalable on AWS**.

---

## 📖 About

DevLab enables learners to practice **HTML, CSS, JavaScript, React, and Tailwind** through hands-on challenges. Submissions are executed and validated in an **isolated headless browser**; learners receive **instant feedback**, **scores**, and **personalized resources**. A simple **forum** fosters collaboration and Q&A.

---

## 🌟 Key Features

- 👤 **Auth & Profiles** — JWT-based auth, user profiles, role flags (user/admin).
- 🧑‍💻 **Monaco Editor Playground** — Real-time code editing with preview.
- 🧪 **Instant Evaluation** — Headless Chrome (Puppeteer) runs custom validation against learner output.
- 🏆 **Challenges & Leaderboard** — Track progress, attempts, and scores.
- 🎯 **Adaptive Recommendations** — Flask microservice returns learning resources based on history.
- 💬 **Discussion Forum** — Post questions, share tips, and discuss solutions.
- 📊 **Analytics** — Progress and usage insights (expandable).
- ☁️ **Cloud-Native** — S3 for assets/CSV, DynamoDB for users/posts, EB/EC2 for API, Amplify for frontend.
- 🔐 **Security-First Defaults** — Env-based secrets, IAM roles, least privilege.

> **Note:** Current evaluator runs on **Node + Puppeteer**. A serverless/Lambda move is on the roadmap.

---

## 🧩 Architecture

<p align="center">
  <a href="docs/architecture1.png">
    <img src="docs/architecture1.png" alt="DevLab AWS Architecture" width="75%">
  </a>
  <br/>
  <sub>High-level AWS layout for DevLab.</sub>
</p>

---
## 🖼️ Demo Walkthrough

> Click any image to view full size. This gallery presents the product flow from sign-up to results.

<table>
  <tr>
    <td align="center" width="33%">
      <a href="docs/registration2.png">
        <img src="docs/registration2.png" alt="Registration" width="95%">
      </a>
      <br/>
      <sub><b>1) Registration</b> — Create an account with basic details.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/loginform2.png">
        <img src="docs/loginform2.png" alt="Login" width="95%">
      </a>
      <br/>
      <sub><b>2) Login</b> — Secure access to your learning workspace.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/landing.png">
        <img src="docs/landing.png" alt="Landing" width="95%">
      </a>
      <br/>
      <sub><b>3) Landing</b> — Welcome page with quick actions & navigation.</sub>
    </td>
  </tr>

  <tr>
    <td align="center" width="33%">
      <a href="docs/Challenges1.png">
        <img src="docs/Challenges1.png" alt="Challenges List" width="95%">
      </a>
      <br/>
      <sub><b>4) Challenges (I)</b> — Browse curated tasks by topic & difficulty.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/Challenges2.png">
        <img src="docs/Challenges2.png" alt="Challenge Details" width="95%">
      </a>
      <br/>
      <sub><b>5) Challenges (II)</b> — View requirements, hints & scoring rules.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/forum.png">
        <img src="docs/forum.png" alt="Forum" width="95%">
      </a>
      <br/>
      <sub><b>6) Forum</b> — Discuss problems, share tips, and get help.</sub>
    </td>
  </tr>

  <tr>
    <td align="center" width="33%">
      <a href="docs/coding_workspace.png">
        <img src="docs/coding_workspace.png" alt="Coding Workspace" width="95%">
      </a>
      <br/>
      <sub><b>7) Coding Workspace</b> — Monaco editor with live preview & tests.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/resource_collection.png">
        <img src="docs/resource_collection.png" alt="Resource Collection" width="95%">
      </a>
      <br/>
      <sub><b>8) Resource Collection</b> — Add optional study links for guidance.</sub>
    </td>
    <td align="center" width="33%">
      <a href="docs/result.png">
        <img src="docs/result.png" alt="Results" width="95%">
      </a>
      <br/>
      <sub><b>9) Results</b> — Instant feedback, pass/fail status, and next steps.</sub>
    </td>
  </tr>
</table>

---
## 🛠 Tech Stack

<div align="center">

<a href="https://react.dev/"><img src="https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=white" alt="React"/></a>
<a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white" alt="Vite"/></a>
<a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/TailwindCSS-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/></a>
<img src="https://img.shields.io/badge/Monaco%20Editor-1f7a8c" alt="Monaco Editor"/>
<br/>
<a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white" alt="Node.js"/></a>
<a href="https://expressjs.com/"><img src="https://img.shields.io/badge/Express-000000?logo=express&logoColor=white" alt="Express"/></a>
<img src="https://img.shields.io/badge/JWT-000000" alt="JWT"/>
<br/>
<a href="https://pptr.dev/"><img src="https://img.shields.io/badge/Puppeteer-40B5A4?logo=puppeteer&logoColor=white" alt="Puppeteer"/></a>
<a href="https://flask.palletsprojects.com/"><img src="https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white" alt="Flask"/></a>
<br/>
<a href="https://aws.amazon.com/dynamodb/"><img src="https://img.shields.io/badge/DynamoDB-4053D6?logo=amazondynamodb&logoColor=white" alt="DynamoDB"/></a>
<a href="https://aws.amazon.com/s3/"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazon-s3&logoColor=white" alt="Amazon S3"/></a>
<br/>
<a href="https://aws.amazon.com/elasticbeanstalk/"><img src="https://img.shields.io/badge/Elastic%20Beanstalk-3B3B3B?logo=amazon-aws&logoColor=white" alt="Elastic Beanstalk"/></a>
<a href="https://aws.amazon.com/amplify/"><img src="https://img.shields.io/badge/AWS%20Amplify-FF9900?logo=awsamplify&logoColor=white" alt="AWS Amplify"/></a>
<a href="https://aws.amazon.com/cloudwatch/"><img src="https://img.shields.io/badge/CloudWatch-FF4F8B?logo=amazon-aws&logoColor=white" alt="CloudWatch"/></a>
<a href="https://aws.amazon.com/cloudtrail/"><img src="https://img.shields.io/badge/CloudTrail-232F3E?logo=amazon-aws&logoColor=white" alt="CloudTrail"/></a>
<a href="https://aws.amazon.com/iam/"><img src="https://img.shields.io/badge/IAM-232F3E?logo=amazon-aws&logoColor=white" alt="IAM"/></a>

</div>

<br/>

<details>
  <summary><b>Frontend</b> — React, Vite/CRA, TailwindCSS, Monaco Editor</summary>
  <ul>
    <li>SPA with route guards and layout shells</li>
    <li>Monaco editor playground with live preview</li>
    <li>Utility-first styling via TailwindCSS</li>
  </ul>
</details>

<details>
  <summary><b>Backend API</b> — Node.js, Express.js, JSON Web Tokens</summary>
  <ul>
    <li>REST endpoints for auth, posts, attempts</li>
    <li>JWT-based sessions and role flags</li>
    <li>Input validation, rate limiting, CORS</li>
  </ul>
</details>

<details>
  <summary><b>Evaluator</b> — Puppeteer (headless Chrome)</summary>
  <ul>
    <li>Runs user HTML/CSS/JS in sandboxed headless Chrome</li>
    <li>Applies whitelisted validation scripts; returns structured results</li>
    <li>Timeouts and resource limits for safety</li>
  </ul>
</details>

<details>
  <summary><b>ML Recommender</b> — Flask (Python)</summary>
  <ul>
    <li>Consumes anonymized attempt history & skill tags</li>
    <li>Returns ranked resources from S3-backed catalog</li>
    <li>Pluggable for embeddings or CF later</li>
  </ul>
</details>

<details>
  <summary><b>Data</b> — DynamoDB & Amazon S3</summary>
  <ul>
    <li><code>users</code>, <code>posts</code>, <code>attempts</code> tables (GSIs for user/challenge lookups)</li>
    <li>S3 for static assets, CSV datasets, screenshots</li>
  </ul>
</details>

<details>
  <summary><b>Infra</b> — Elastic Beanstalk, Amplify, CloudWatch/CloudTrail, IAM</summary>
  <ul>
    <li>EB for Node API & Flask; Amplify for static frontend</li>
    <li>CloudWatch logs/metrics; CloudTrail auditing</li>
    <li>IAM roles (least privilege) for DynamoDB/S3 access</li>
  </ul>
</details>

<!-- Quick summary table for skimmers -->
| 🧩 Layer           | 🛠️ Stack |
|--------------------|----------|
| **Frontend**       | React · Vite/CRA · TailwindCSS · Monaco Editor |
| **Backend API**    | Node.js · Express.js · JWT |
| **Evaluator**      | Puppeteer (headless Chrome) |
| **ML Recommender** | Flask (Python) |
| **Data**           | DynamoDB (Users, Posts, Attempts) · Amazon S3 (assets/CSV) |
| **Infra**          | Elastic Beanstalk (API & Flask) · Amplify (Frontend) · CloudWatch/CloudTrail · IAM |

---

## 📚 References

### Research & Articles

- [Springer Chapter](https://link.springer.com/chapter/10.1007/978-981-97-1329-5_28)
- [IEEE Xplore — Document 10497289](https://ieeexplore.ieee.org/document/10497289)
- [IEEE Xplore — Document 10426375](https://ieeexplore.ieee.org/abstract/document/10426375)
- [arXiv Preprint](https://arxiv.org/abs/2307.08705)
- [Springer Chapter](https://link.springer.com/chapter/10.1007/978-3-030-60036-5_3)
- [Journal of Cloud Computing (SpringerOpen)](https://journalofcloudcomputing.springeropen.com/articles/10.1186/s13677-019-0134-y)

> *Some resources (Springer, IEEE Xplore) may require institutional access.*

---

### AWS Services Documentation
- [Amazon EC2 — Concepts](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html)
- [Amazon CloudWatch — Docs](https://docs.aws.amazon.com/cloudwatch/)
- [AWS Elastic Beanstalk — Docs](https://docs.aws.amazon.com/elasticbeanstalk/)
- [Amazon DynamoDB — Docs](https://docs.aws.amazon.com/dynamodb/)
- [AWS DevOps Blog — Complete CI/CD with CodeCommit, CodeBuild, CodeDeploy & CodePipeline](https://aws.amazon.com/blogs/devops/complete-ci-cd-with-aws-codecommit-awscodebuild-aws-codedeploy-and-aws-codepipeline/)
- [Amazon S3 — Docs](https://docs.aws.amazon.com/s3/)
- [AWS Amplify — Docs](https://docs.amplify.aws/)
- [AWS IAM — Docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
