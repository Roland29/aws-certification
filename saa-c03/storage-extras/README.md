# Storage Extras

<details>
 <summary><i>Menu</i></summary>

- [Snow Family](#snow-family)
- [FSX](#fsx)
- [Hybrid Cloud Storage](#hybrid-cloud-storage)
- [Transfer Family](#transfer-family)
- [DataSync](#datasync)
</details>

---
## Snow Family
- Data migration / Edge computing
  - snowcone
      - 8 TB HDD | 14 TB SSD
  - snowball
    - 80 TB usable
    - Edge
      - up to 80 TB of usable HDD storage
      - 40 vCPUs
      - 1 TB of SATA SSD storage
      - and up to 40 Gb network connectivity 
      - To address large scale data transfer and pre-processing use cases
    - Can be copied into the S3 bucket
  - snowmobile
    - 100 PB capacity

---
## FSX
- Windows file server 
- Lustre
  - easy and cost-effective to launch and run the world’s most popular high-performance file system
  - transparently presents S3 objects as files and allows you to write changed data back to S3
  - HPC (High Performance computing)
  - Seamless integration with S3
  - Scratch file system
  - Persistent file system
- NetApp ONTAP
  - Compatible with windows, linux & mac 
  - NFS, SMB, ISCI protocol (ONTAP | NAS)
- OpenZFS
  - Compatible with windows, linux & mac
  - NFS

---
## Hybrid Cloud Storage
- Storage Cloud Native
  - Block
  - File
  - Object
- Storage Gateway
  - S3 file gateway
  - FSx file gateway
  - Volume gateway
    - Cached Volume
    - Stored Volume
  - Tape gateway
  - Hardware Gateway

---
## Transfer Family
- FTP
- FTPS
- SFTP

To S3 or EFS

---
## DataSync
- Move large amount of data to and from
- Can synchronize to
- Replication task
- File permission and metadata are preserved
- outputs:
  - s3
  - EFS
  - Fsx windows
  - Fsx Lustre
  - Fsx OpenZFS
  - Fsx NetApp ONTAP
