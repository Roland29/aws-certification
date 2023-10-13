Disaster & Recovery
-

- Recovery Point Objective (RPO)
  - how often backups
- Recovery Time Objective (RTO)
  - Time to restore the system

Strategies
-
- Backup & Restore (High RPO)
- Pilot Light
- Warm standby
- Multi Site / Hot Site Approach
- AWS Multi Region

DMS - Database Migration Service
-
- Must create EC2 to perform the replication
- If from SQL Server to Mysql need of AWS Schema Conversion Tool (SCT)
- Continuous Replication
- Multi-AZ
- RDS & Aurora MySQL Migration
  - RDS MySQL to Aurora
    - snapshot
    - read replica
  - External MySQL to Aurora
    - Use Percona XtraBackup to create a file backup in S3
- Enables to migrate data from supported sources to
  - relational databases
  - data warehouses
  - streaming platforms (Kinesis, ...)
  - other data stores in AWS cloud

Migrate On-Premise with AWS
-
- VM import/export
- Application Discovery service
- DMS
- Server Migration Service (SMS)

AWS Backup
-
- Fully managed service
- Centrally manage and automate backups across AWS services
- Vault lock policy (WORM) write once read many

Application Discovery Service
-
- 2 types of migrations
  - Agentless Discovery
  - Agent-based Discovery

Application Migration Service (MGM)
-
- Migrate application to AWS

VMware cloud on AWS
-

Transfer large amount of data
-
- Over the internet / Site-to-Site VPN
- Over direct connect (1 Gbps)
- Over snowball
- For on-going replication / transfers