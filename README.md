# Ali Achille Traoré

**DevOps Engineer | Full-Stack Software Engineer (MERN)**

I build cloud infrastructure, deployment workflows, and full-stack web applications.

Most of my production DevOps work has been delivered in private client and enterprise environments. This GitHub highlights my public software engineering projects, selected technical work, and the hands-on portfolio I use to demonstrate how I design, build, and troubleshoot systems.

## Core Areas

- Full-Stack Software Engineering (MERN)
- Cloud Infrastructure & Automation
- CI/CD & Deployment Reliability
- Containerization & Orchestration
- Infrastructure as Code
- Monitoring, Logging & Troubleshooting

## Public Work on GitHub

### Restaurant Deals
A full-stack MERN application built around restaurant promotions, user workflows, and role-based access.

### Selected Technical Practice
Additional repositories on this profile reflect technical practice across web development, JavaScript, Java, and deployment-related work.

## Background

I bring 6+ years of DevOps experience across cloud infrastructure, CI/CD, containerized environments, Infrastructure as Code, monitoring, and production support. My public GitHub is centered on full-stack software engineering with the MERN stack, along with selected technical work that reflects my broader background in automation, systems, and deployment.

## Engineering Architecture (Flow-Based)

### Runtime Flow (MERN)
How the application serves users in production (request → auth → data → response):

```mermaid
flowchart LR
    U[Users] -->|HTTPS| FE["React + TypeScript UI<br/>Vite build + Tailwind styling"]
    FE -->|REST/JSON| API["Node.js + Express API<br/>TypeScript"]
    FE -->|Send token| AUTH[JWT Auth]
    API -->|Verify token| AUTH
    AUTH -->|Enforce roles| AC["Access Control - RBAC"]
    API --> AC
    AC --> DB[(MongoDB)]
    API --> OBS["Logs / Metrics / Traces"]
```

### Delivery Flow (DevOps)
How changes move from commit → pipeline → container → infrastructure → deployment → monitoring:

```mermaid
flowchart TB
    Dev[Developer] -->|push| SCM[Git repository]
    SCM --> CI["Jenkins Pipeline<br/>Jenkinsfile = pipeline-as-code"]

    CI --> QA["Lint + Unit/Integration Tests"]
    CI --> Build["Build / Bundle<br/>TypeScript + Vite"]
    Build --> Img["Docker Build<br/>Immutable images"]
    Img --> Reg[Container Registry]

    CI --> IaC["Terraform Plan/Apply<br/>Infrastructure as Code"]
    IaC --> Cloud["Cloud Environment<br/>AWS / Azure"]

    Reg --> Deploy["Deploy/Update Services<br/>rolling updates"]
    Deploy --> Cloud

    Cloud --> Verify["Health Checks + Rollback Hooks"]
    Cloud --> Monitor["Monitoring + Alerting"]
```

## Tech Stack (Mapped to Responsibilities)

This stack is organized into two systems: **runtime** (how requests are handled) and **delivery** (how changes ship safely).

### Runtime (Build the Product)

Application
- **React + TypeScript**: component-driven UI with type safety
- **Vite**: fast local development and production bundling
- **Tailwind CSS**: consistent styling and fast UI iteration
- **Node.js + Express + TypeScript**: REST APIs, middleware, validation, and backend workflow handling
- **JWT + RBAC**: stateless authentication and server-side access control

Data and Storage
- **MongoDB + Mongoose**: document data model for MERN applications
- **PostgreSQL / RDS**: relational workloads and managed database operations
- **DynamoDB / Redshift / Aurora / Oracle**: broader database exposure across cloud and enterprise environments
- **S3 / object storage concepts**: static assets, storage integration, and cloud-based data workflows

Operations
- **Logging / metrics / tracing**: production visibility, troubleshooting, and operational feedback loops

### Delivery (Ship Reliability)

CI/CD and Automation
- **Jenkins / GitHub Actions / GitLab CI / Azure DevOps**: pipeline automation, build orchestration, and deployment workflows
- **Terraform / CloudFormation / Ansible**: Infrastructure as Code, configuration automation, and repeatable environments

Containers and Platforms
- **Docker / Docker Compose**: consistent packaging across development, test, and production
- **Kubernetes / OpenShift**: container orchestration and platform operations
- **Linux / Bash / Python**: scripting, automation, and systems troubleshooting

Cloud Platforms
- **AWS / Azure**: compute, networking, storage, IAM, and managed cloud services

## Certifications

[![AWS DevOps Engineer – Professional](https://img.shields.io/badge/AWS-DevOps_Engineer_Professional-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://www.credly.com/users/ali-achille-traore)

[![AWS Cloud Practitioner](https://img.shields.io/badge/AWS-Cloud_Practitioner-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)](https://www.credly.com/users/ali-achille-traore)

[![Google IT Support Professional Certificate](https://img.shields.io/badge/Google-IT_Support-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://www.credly.com/users/ali-achille-traore)

[![IBM Software Engineering Essentials](https://img.shields.io/badge/IBM-Software_Engineering_Essentials-1261FE?style=for-the-badge&logo=ibm&logoColor=white)](https://www.credly.com/users/ali-achille-traore)

**View all badges:** [Credly Profile](https://www.credly.com/users/ali-achille-traore)

## Connect

- [LinkedIn](https://linkedin.com/in/ali-achille-traore)
- [Email](mailto:ali.achille.traore@gmail.com)
- [GitHub](https://github.com/traliach)

## Open To

DevOps, Cloud, and Full-Stack Software Engineering opportunities.
