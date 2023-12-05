# Integration & Messaging

<details>
 <summary><i>Menu</i></summary>

- [SQS](#sqs)
- [SNS](#sns)
- [Kinesis Data Agent](#kinesis-agent)
- [Kinesis Data Streams](#kinesis-data-streams)
- [Kinesis Data Firehose](#kinesis-data-firehose)
- [Kinesis Data Analytics](#kinesis-data-analytics)
- [Kinesis Video Streams](#kinesis-video-streams)
- [Amazon MQ](#amazon-mq)
</details>

---
## SQS
- Queue model
- Retention 4 days to 14 days
- low latency (<10ms on pub/receive)
- Limit of 256 KB
- security
  - Encryption
    - in-flight using https
    - at-rest using KMS keys
    - Client-side
  - Access control
    - IAM policies
  - SQS Access Policies
    - similar to S3 bucket policies
    - Useful for cross-account access to SQS queues
    - Useful for allowing other services (SNS, S3...) to write to an SQS queue
- Visibility timeout
- Long polling
  - LongPolling decreases the number of API calls made to SQS while increasing the efficiency and reducing latency of your application
- FIFO
  - 3,000 messages per second with batching
  - 300 messages per second without batching (300 send, receive, or delete operations per second)
  - name end with the __.fifo__ suffix
- Auto-scaling group (ASG)
![SQS delay](../../images/sqs-delay-queues-diagram.png)
- SQS extended client (__only with aws sdk java__)
  - use S3 message up to 2GB

---
## SNS
- Pub/sub model
- security
  - Encryption
    - in-flight using https
    - at-rest using KMS keys
    - Client-side
  - Access control
    - IAM policies
  - SNS Access Policies
    - similar to S3 bucket policies
    - Useful for cross-account access to SNS queues
    - Useful for allowing other services (S3...) to write to an SNS queue
- Topic Publish
- Direct Publish
- SNS + SQS -> Fan Out
- Kinesis Data Firehose (KDF)
- FIFO
- __Message Filtering__

---
## Kinesis Agent
- stand-alone Java software application that offers an easy way to collect and send data to
  - Kinesis Data Streams
  - Kinesis Firehose

---
## Kinesis Data Streams
- Capture, process, and store data streams
- massively scalable and durable real-time data streaming service
  - can continuously capture gigabytes of data per second from hundreds of thousands of sources
- Can scale # of shards
- shared (2MB/sec per shard all consumers)
- enhanced fan-out (2MB/sec per shard per consumer)
- Capacity Modes
  - Provisioned mode
  - On-demand mode
- Can only have as many consumers as shards
- Batch messages
- Operations
  - Shared splitting 1 -> 2
  - Shared merging 2 -> 1 

---
## Kinesis Data Firehose
- Load data streams into AWS data stores
- Put upt to 1 MB
- read batch writes
- Buffer
- Flush
- Input:
  - only one ?
- outputs:
  - S3
  - Redshift
  - OpenSearch
  - Splunk
![KDF](../../images/Amazon-Kinesis-Data-Firehose.png)

---
## Kinesis Data Analytics
- Analyze data streams with SQL or Apache Flink
- Goto analytic [here](../data-analytics/README.md#kinesis-data-analytics)

---
## Kinesis Video Streams
- Capture, process, and store video streams

---
## Amazon MQ
- RabbitMQ
- ActiveMQ