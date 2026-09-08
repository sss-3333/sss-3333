# Hey, I'm Safaa 👋

### DevOps Engineer

Building cloud infrastructure on AWS with Terraform, Docker, and CI/CD -
learning by shipping real, working deployments rather than just tutorials.

---

### Tech Stack

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-000000?style=for-the-badge&logo=linux&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

### Featured Project

#### 🚀 [Trackance - Client Project Tracker on AWS ECS](https://github.com/sss-3333/ECS-project)

A containerised Node.js app deployed to ECS Fargate, provisioned entirely
with Terraform - built end-to-end, from a manual ClickOps setup through to
a fully automated CI/CD pipeline.

- 5 reusable Terraform modules (VPC, ECR, ACM, ALB, ECS), with GitHub OIDC
  authentication and the container registry split into their own
  independent Terraform state, so a full teardown of the app
  infrastructure never removes the pipeline's own credentials or image
- Hand-built least-privilege IAM policy for CI/CD - no `AdministratorAccess` —
  tested by locally assuming the actual role and running `terraform plan`
  and `destroy` against it until both came back clean
- Immutable ECR image tags, deployed by digest via a Terraform data source
  that always resolves to the most recently pushed image automatically
- Multi-stage, distroless, non-root Dockerfile
- 4 GitHub Actions pipelines: build & push, PR-gated plan, deploy with a
  post-deploy health check, and a manually-confirmed destroy
- Custom domain with a DNS-validated ACM certificate and a forced
  HTTP → HTTPS redirect

`ECS Fargate` `Terraform` `Docker` `GitHub Actions` `OIDC` `ECR` `ALB` `ACM` `Route 53` `VPC`

---
### Mini Projects
 
- [Docker Multi-Container Apps](https://github.com/sss-3333/docker-journey) — Flask + MySQL, Flask + Redis, Docker Compose
- [WordPress on EC2 via Terraform](https://github.com/sss-3333/terraform-journey/tree/main/projects/DeployWordPress) — bash user-data provisioning
- [NGINX on EC2 via Terraform](https://github.com/sss-3333/terraform-journey/tree/main/projects/cloud-init) — cloud-init provisioning

---

### Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/safaa-sheikh-7283b5219)
