SQS
-
---
## Queue model
 Retention 4 days to 14 days
- low latency (<10ms on pub/receive)
- Limit of 256 KB
- security
  - Encryption
  - Access control
  - SQS Access Policies
- Visibility timeout
- Long polling
- FIFO
  - 3,000 messages per second with batching
  - 300 messages per second without batching (300 send, receive, or delete operations per second)
  - name end with the __.fifo__ suffix
- Auto-scaling group (ASG)

---
## SNS

---
## Pub/sub model
 security
    - Encryption
    - Access control
    - SQS Access Policies
- Topic Publish
- Direct Publish
- SNS + SQS -> Fan Out
- Kinesis Data Firehose (KDF)
- FIFO
- Message Filtering

---
## Kinesis Data Streams

- massively scalable and durable real-time data streaming service
  - can continuously capture gigabytes of data per second from hundreds of thousands of sources
- Can scale # of shards
- shared (2MB/sec per shard all consumers)
- enhanced fan-out (2MB/sec per shard per consumer)
- Capacity Modes
  - Provisioned mode
  - On-demand mode

---
## Kinesis Data Firehose

- Put upt to 1 MB
- read batch writes
- Buffer
- Flush
- outputs:
  - S3
  - Redshift
  - OpenSearch
  - Splunk

---
## Kinesis Data Analytics


---
## Kinesis Video Streams


---
## Amazon MQ

- RabbitMQ
- ActiveMQ