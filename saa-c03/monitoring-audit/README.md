CloudWatch
-
- Streams Metric
- Logs
  - Insight
  - S3 export
    - up to 12 hours
  - Subscription
    - real-time to
      - lambda
      - kinesis data stream
      - kinesis data firehose
    - filter
- CloudWatch logs Agent
  - only logs
- Cloudwatch Unified Agent
  - logs + information of server (CPU, Disk, RAM, Nestat, swap)
- Alarms

EventBridge
-
- Schedule cron jobs
- cross account capability

Cloudwatch container Insight
-
- using containerized version of cloudwatch agent to discover containers

Cloudwatch lambda Insight
-

Cloudwatch Contributor Insight
-
- Identify the heaviest work network users

Cloudwatch Application Insight
-
- Automated dashboard to monitor applications

CloudTrail
-
- GET history of events / API calls made within your AWS Account by:
  - SDK
  - Console
  - CLI
  - AWS services
- Events
  - Management Events
    - Read events
    - Write events
    - enable By default
  - Data events
    - disable By default
  - Insights Events
- Events Retention
  - Stored 90 days
  - Send to S3

AWS Config
-
- config rules per region
- could add remediation
- Can send Notifications