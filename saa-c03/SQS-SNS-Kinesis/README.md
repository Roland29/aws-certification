SQS
-
Queue model
- Retention 4 days to 14 days
- low latency (<10ms on pub/receive)
- Limit of 256 KB
- security
  - Encryption
  - Access control
  - SQS Access Policies
- Visibility timeout
- Long polling
- FIFO
- Auto-scaling group (ASG)

SNS
-
Pub/sub model
- security
    - Encryption
    - Access control
    - SQS Access Policies
- Topic Publish
- Direct Publish
- SNS + SQS -> Fan Out
- Kinesis Data Firehose (KDF)
- FIFO
- Message Filtering

Kinesis
-
Real-time streaming model
- Data Streams
  - Can scale # of shards
  - shared (2MB/sec per shard all consumers)
  - enhanced (2MB/sec per shard per consumer)
  - Capacity Modes
    - Provisioned mode
    - On-demand mode
- Data Firehose
  - Put upt to 1 MB
  - read batch writes
  - Buffer
  - Flush
- Data Analytics
- Video Streams

Amazon MQ
-
- RabbitMQ
- ActiveMQ