# Containers on AWS

<details>
 <summary><i>Menu</i></summary>

- [Docker](#docker)
- [ECS](#amazon-ecs)
- [ECR](#amazon-ecr)
- [EKS](#amazon-eks)
- [App Runner](#app-runner)
</details>

---
## Docker


---
## Amazon ECS
- EC2 Launch type
  - manage EC2
- Fargate Launch type
  - serverless
- IAM Roles
  - EC2 instance profile
  - ECS Task Role
- Load Balancer Integration
- Data Volumes
  - EFS
- Auto scaling
  - CPU
  - RAM
  - Metric from ALB

---
## Amazon ECR
- Elastic container registry
- private and public repository
- public gallery: https://gallery.ecr.aws
- IAM permission

---
## Amazon EKS
- kubernetes
- Node Types
  - Managed Node Groups
  - Self-Managed Nodes
  - AWS Fargate
- Data Volumes
  - StorageClass in manifest
  - support for:
    - EBD
    - EFS
    - FSx lustre
    - FSx NetApp ONTAP

---
## App Runner

---
## ECS Task 
- Strategies
  - binpack
  - spread
  - random
- Placement constraint
  - distinctInstance
  - memberOf
