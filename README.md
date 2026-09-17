# 🚀 Claim Zero — AWS Cloud & DevOps Project

> **A 4-day hands-on introduction to Cloud, DevOps, Docker, AWS, Infrastructure as Code and CI/CD.**

Claim Zero was a **4-day practical course** where I progressed from setting up a complete development environment to deploying a containerised React application on AWS and automating the deployment process with CI/CD.

---

## 🗓️ 4-Day Journey

### 🛠️ Day 1 — Introduction & Environment Setup

The first day focused on understanding the course, the tools we would be using, and setting up the development environment.

I installed and configured the main tools required for the project:

* **Node.js** — JavaScript runtime
* **Git** — version control
* **Docker** — containerisation
* **AWS CLI** — interacting with AWS
* **Terraform** — Infrastructure as Code
* **VS Code** — development environment

We also covered the basics of how these technologies fit together in a modern DevOps workflow.

```text
Developer
    │
    ├── Git
    ├── Node.js
    ├── Docker
    ├── AWS CLI
    └── Terraform
            │
            ▼
          AWS
```



---

### 🐳 Day 2 — Docker & AWS Deployment

Day 2 moved from setup into practical deployment.

I worked with the React application and packaged it into a Docker container using a multi-stage Dockerfile.

The application was built locally and tested through Docker before being prepared for AWS.

```text
React Application
       ↓
   Docker Build
       ↓
 Docker Image
       ↓
 Local Container
       ↓
 localhost:8080
```

The Docker image was then pushed to **Amazon ECR** and deployed using **Amazon ECS running on EC2**.

```text
Docker Image
     ↓
Amazon ECR
     ↓
Amazon ECS
     ↓
EC2
     ↓
Live Application
```



---

### 🏗️ Day 3 — Terraform & Infrastructure as Code

Day 3 focused on **Terraform** and learning how cloud infrastructure can be created and managed through code.

Instead of manually configuring every AWS resource, Terraform was used to define the infrastructure.

```text
Terraform
    ↓
AWS Resources
    ↓
ECS + EC2
    ↓
Application
```

I worked with resources including:

* ECS
* EC2
* IAM
* Security Groups
* CloudWatch
* Networking

The Terraform workflow included:

```bash
terraform init
terraform validate
terraform plan
terraform apply
```


---

### 🔄 Day 4 — GitHub & CI/CD

The final day focused on automating the deployment process.

The project was connected to **GitHub**, with AWS CodePipeline and CodeBuild handling the CI/CD workflow.

```text
GitHub
   ↓
CodePipeline
   ↓
CodeBuild
   ↓
Docker Build
   ↓
Amazon ECR
   ↓
Amazon ECS
   ↓
Updated Application
```

A change pushed to the `main` branch could trigger the pipeline.

CodeBuild built the Docker image and pushed it to ECR, while CodePipeline handled the deployment to ECS.



---

# 🏗️ Final Architecture

```text
                    GitHub
                      │
                      ▼
                CodePipeline
                      │
                      ▼
                 CodeBuild
                      │
                 Docker Build
                      │
                      ▼
                    ECR
                      │
                      ▼
                    ECS
                      │
                      ▼
                    EC2
                      │
                      ▼
               Docker Container
                      │
                      ▼
                Nginx + React
                      │
                      ▼
               Live Application
```

---

# 🛠️ Technologies Used

| Category        | Technologies            |
| --------------- | ----------------------- |
| Development     | VS Code, Node.js        |
| Version Control | Git, GitHub             |
| Containers      | Docker, Nginx           |
| Cloud           | AWS, ECS, EC2, ECR      |
| Infrastructure  | Terraform               |
| CI/CD           | CodePipeline, CodeBuild |
| Monitoring      | CloudWatch              |
| CLI             | AWS CLI                 |

---

# 🎯 Skills Demonstrated

Across the four days, I gained practical exposure to:

* Development environment setup
* Git and version control
* Docker containerisation
* Building and running Docker images
* Amazon ECR
* Amazon ECS and EC2
* AWS IAM and security configuration
* Terraform Infrastructure as Code
* AWS CodeBuild
* AWS CodePipeline
* GitHub integration
* Automated application deployment
* Basic Cloud and DevOps workflows

---

# 📸 Project Screenshots

The following screenshots document the progression of the project:

**Day 1 — Environment Setup**
Tools installed and configured.

**Day 2 — Docker & AWS**
Application containerised and deployed to AWS.

**Day 3 — Terraform**
AWS infrastructure created and managed through code.

**Day 4 — CI/CD**
GitHub connected to AWS and automated deployment successfully running.

---

# ✅ Final Result

Over four days, I progressed from **setting up the tools required for cloud development** to deploying a React application on AWS with an automated CI/CD workflow.

```text
DAY 1
Setup & Fundamentals
        ↓
DAY 2
Docker & AWS Deployment
        ↓
DAY 3
Terraform Infrastructure
        ↓
DAY 4
GitHub & CI/CD
        ↓
FINAL
Automated AWS Deployment
```

The project gave me practical experience across the development and deployment lifecycle, combining **Git, Docker, AWS, Terraform and CI/CD** into one working project.

---

### 👨‍💻 Claim Zero

**4-Day AWS Cloud & DevOps Project**

**Git · Node.js · Docker · AWS · ECR · ECS · EC2 · Terraform · GitHub · CodeBuild · CodePipeline**
