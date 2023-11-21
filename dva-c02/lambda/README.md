# Lambda

<details>
 <summary><i>Menu</i></summary>

- [Lambda](#lambda-1)
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
- Types
  - Asynchronous
    - can use a DLQ
  - Synchronous
  - Events source mappings
    - Kinesis Data Streams & DynamoDB Streams
      - One Lambda invocation per stream shard
      - If you use parallelization, up to 10 batches processed per shard simultaneously
    - SQS Standard
      - Lambda adds 60 more instances per minute to scale up
      - Up to 1000 batches of messages processed simultaneously
    - SQS FIFO
      - Messages with the same GroupID will be processed in order
      - The Lambda function scales to the number of active message groups
- Event Object
- Context Object
- Destinations
  - for success
  - failure
- Concurrency
  - Up to 1000
  - Provisioned
  - Reserved

---
## Lambda + ALB
- Need to create a Target Group for the ALB to use Lambda
- Multi-Headers values
  - if enable on ALB -> transform in list inside  JSON


---
## Lambda X-Ray
- daemon address

---
## Edge function
- Cloudfront function 
  - million requests/second
  - viewer request and response
  -   execution time < 1ms
- lambda@edge
  - 1000s requests/second
  - viewer request and response
  - origin  request and response
  - execution time 5 to 10 seconds