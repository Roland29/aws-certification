# Lambda

<details>
 <summary><i>Menu</i></summary>

- [Lambda](#lambda)
</details>

---
## Lambda
- short executions
- on-demand
- scaling is automated
- very cheap
- Limits
  - Execution
    - 128 MB to 10 GB
    - 15 min
    - env variables 4 KB
    - disk capacity 512 MB to 10 GB
    - Concurrency executions: 1000
  - Deployment
    - 50 MB compressed (.zip)
    - 250 MB uncompressed
    - Can use /tmp directory to load other files at startup
    - env variables 4 KB
- Lambda@Edge vs CloudFront function
- Lambda in VPC
- RDS Proxy
- Layer
  - a ZIP archive that contains libraries, a custom runtime, or other dependencies
  - let you keep your deployment package small
  - can use up to 5 layers at a time
- security IAM role
![VPC lambda](../../images/vpcLambda.png)
- Price 0.06$ per hour
