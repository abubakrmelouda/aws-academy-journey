# Module 7: Storage Services.

Completed: November 20, 2025
Knowledge Check: 70/100
Lab Score: 25/25 (100%)
Time Spent: 8 hours

## Key Concepts:

1. **Amazon EBS (Elastic Block Store):**
   - **Block-level Storage:** Provides persistent block storage volumes for Amazon EC2 instances
   - **Instance-attached Storage:** Directly attached to EC2 instances for low-latency access
   - **Snapshot Capability:** Create point-in-time backups that can be restored across regions
   - **Volume Types:** SSD (gp2, io1) for high I/O, HDD (st1, sc1) for throughput/cold storage

2. **Amazon S3 (Simple Storage Service):**
   - **Object Storage:** Store and retrieve any amount of data at any time from anywhere
   - **11 Nines Durability:** Designed for 99.999999999% durability
   - **Storage Classes:** Standard, Intelligent-Tiering, Standard-IA, One Zone-IA, Glacier, Glacier Deep Archive
   - **Global Bucket Names:** Bucket names must be globally unique and DNS-compliant

3. **Specialized Storage Services:**
   - **Amazon EFS (Elastic File System):** Scalable, shared file storage for Linux workloads
   - **Amazon S3 Glacier:** Secure, durable, low-cost storage for data archiving and backup
   - **Amazon S3 Glacier Deep Archive:** Lowest-cost storage for long-term retention (7-10+ years)

## Module Completion
- 5 instructional videos including EBS/S3/EFS console demonstrations completed
- Reviewed Learner Guide
- **Completed Lab 4: Working with EBS (25/25)**
- **Achieved 70% on Knowledge Check**
- Explored EBS, S3, EFS and Glacier consoles
- Participated in storage case activities

## Hands-On Lab: Working with EBS

### **Lab Objectives Achieved:**
1. **Created EBS Volume:**
   - Successfully created 1GB General Purpose SSD (gp2) volume
   - Selected appropriate Availability Zone matching EC2 instance
   - Applied proper tagging for resource management

2. **Attached and Configured Volume:**
   - Attached EBS volume to running EC2 instance
   - Used correct device naming (/dev/sdf)
   - Formatted volume with ext3 filesystem
   - Mounted volume to directory structure

3. **Snapshot Management:**
   - Created snapshot of EBS volume
   - Restored snapshot to create new volume
   - Verified data integrity after restoration

### **Lab Performance:**
**Score:** 25/25 (100%)
- **Task 1:** EBS volume created correctly (5/5)
- **Task 2:** Volume attached successfully (5/5)
- **Task 3:** Volume mounted and accessible (5/5)
- **Task 4:** Snapshot created successfully (5/5)
- **Task 5:** Snapshot restored correctly (5/5)

### **Key Learnings from EBS Lab:**
1. **Volume Creation Process:**
   - Importance of selecting matching Availability Zone with EC2 instance
   - Proper volume type selection based on workload requirements
   - Encryption options for data security at rest

2. **Volume Management:**
   - Device naming conventions in Linux (/dev/sdf, /dev/sdg, etc.)
   - Filesystem creation and mounting procedures
   - Permission configuration for mounted volumes

3. **Snapshot Best Practices:**
   - Incremental backup nature of EBS snapshots
   - Cross-region snapshot copying for disaster recovery
   - Snapshot restoration and volume resizing capabilities

## Architecture Diagrams

### Diagram 1: AWS Storage Services Overview

```mermaid
graph TB
    A[AWS Storage Services] --> B[Block Storage]
    A --> C[Object Storage]
    A --> D[File Storage]
    A --> E[Archive Storage]
    A --> F[Hybrid Storage]
    
    B --> B1[Amazon EBS<br/>Elastic Block Store]
    B --> B2[EC2 Instance Store<br/>Temporary Storage]
    
    C --> C1[Amazon S3<br/>Simple Storage Service]
    C --> C2[Amazon S3 Glacier<br/>Archive Storage]
    
    D --> D1[Amazon EFS<br/>Elastic File System]
    D --> D2[FSx for Windows<br/>Windows File Shares]
    D --> D3[FSx for Lustre<br/>High-Performance Computing]
    
    E --> E1[S3 Glacier Deep Archive<br/>Long-term Retention]
    E --> E2[AWS Backup<br/>Centralized Backup]
    
    F --> F1[Storage Gateway<br/>Hybrid Cloud]
    F --> F2[DataSync<br/>Data Transfer]
