# Other AWS Services

<details>
 <summary><i>Menu</i></summary>

- [CloudFormation](#cloudformation)
- [SES](#simple-email-service-ses)
- [Pinpoint](#amazon-pinpoint)
- [Systems Manager](#systems-manager)
- [Cost Explorer](#cost-explorer)
- [AWS Compute Optimizer](#aws-compute-optimizer)
- [Elastic Transcoder](#elastic-transcoder)
- [Batch](#batch)
- [AppFlow](#appflow)
- [Amplify](#amplify)
- [Trusted Advisor](#aws-trusted-advisor)
</details>

---
## CloudFormation
- Infrastructure as code
- Estimate cost
- Stack designer

---
## Simple Email Service (SES)
- Fully managed service to send emails securely, globally and at scale

---
## Amazon Pinpoint
- scalable 2-way (outbound/inbound) marketing communication service
- Supports:
  - email
  - sms
  - push
  - voice
  - in-app messaging
- Create message template
- schedule delivery
- highly-targeted segments
- full campaigns

---
## Systems Manager
- System Session Manager (SSM)
  - Allows to start a secure shell on your EC2 and on-premises servers
  - No SSH access, bastion host 
  - No port 22 needed
- Run Command
  - run cmd across multiple instances
  - output to S3, cloudWatch
  - notification sns eventBridge
- Patch Manager
  - Maintenance Windows
  - OS update, applications updates
  - on-demand or schedule
  - scan instances and generate patch compliance report
- Maintenance Windows
- Automation
  - Runbook

---
## Cost Explorer
- Visualize, understand and manage your AWS costs and usage over time
- Forecast usage up to 12 months based on previous usage

---
## AWS Compute Optimizer
- Recommends optimal AWS Compute resources for your workloads to reduce costs and improve performance by using machine learning

---
## Elastic Transcoder
- convert media files stored in S3 into media files in the formats required by consumer playback devices (phones, etc...)

---
## Batch
- No time limit
- Any runtime as long as packaged as a Docker
- Rely on EBS / instance store for disk space
- Relies on EC2

---
## AppFlow
- Securely transfer data between SaaS application and AWS

---
## Amplify
- Web and mobile application

---
## AWS Trusted Advisor
- checks for Amazon EC2 Reserved Instances that are scheduled to expire or have expired