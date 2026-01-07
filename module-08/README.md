# Module 8: Database Services-

**Completed:** November 6, 2025  
**Knowledge Check:** 80/100  
**Lab Score:** 15/20 (75%)  
**Time Spent:** 5 hours

##  Key Concepts:

1. **Amazon RDS - Managed Relational Databases:**
   - **Fully Managed Service:** AWS handles provisioning, patching, backup, recovery, and scaling
   - **Multi-AZ Deployments:** Automatic synchronous replication across Availability Zones for high availability
   - **Supported Engines:** MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Amazon Aurora
   - **Read Replicas:** Scale read operations with asynchronous replicas

2. **Amazon DynamoDB - NoSQL Database Service:**
   - **Serverless NoSQL:** Fully managed, key-value and document database
   - **Single-Digit Millisecond Latency:** Consistent performance at any scale
   - **Automatic Scaling:** Throughput capacity scales automatically with application traffic
   - **Global Tables:** Multi-region, multi-active replication for global applications

3. **Specialized Database Services:**
   - **Amazon Aurora:** MySQL/PostgreSQL-compatible with enterprise performance at open-source cost
   - **Amazon Redshift:** Fully managed data warehouse for petabyte-scale analytics
   - **Database Migration:** AWS Database Migration Service for seamless migration to AWS

## Module Completion
- Completed 5 videos including RDS/DynamoDB console demonstrations
- Reviewed Learner Guide
- **Completed Lab 5: Build a Database Server**
- **Achieved 80% on Knowledge Check**
- Explored RDS and DynamoDB consoles
- Participated in database case study activities

## Hands-On Lab: Build a Database Server

### **Lab Objectives Achieved:**
1. **Database Security Configuration:**
   - Configured security group for database access
   - Set up proper inbound rules for database connectivity
   - Implemented network isolation in private subnet

2. **RDS Instance Creation:**
   - Created DB subnet group for multi-AZ deployment
   - Configured MySQL database instance with proper parameters
   - Set up storage, backup, and maintenance settings

3. **Application Integration:**
   - Successfully connected application to RDS database
   - Verified database connectivity and query execution
   - Tested application functionality with live database

### **Lab Performance:**
**Score:** 15/20 (75%)
- **Task 1:** Security Group created 
- **Task 2:** DB subnet group created correctly
- **Task 3:** DB created successfully
- **Task 4:** App connected to DB successfully

### **Challenges and Solutions:**
**Challenge:** Task 1 security group configuration issues
**Learning:** Proper security group configuration is critical for database access control
**Solution:** Needed to ensure security groups allow appropriate inbound traffic from application servers

### **Key Learnings from RDS Lab:**
1. **Database Security:**
   - Importance of network isolation in private subnets
   - Security group configuration for controlled access
   - Encryption options for data at rest and in transit

2. **RDS Configuration:**
   - Instance class selection based on workload requirements
   - Storage allocation and type selection
   - Backup retention and automated snapshot management

3. **High Availability:**
   - Multi-AZ deployment for automatic failover
   - Read replicas for scaling read operations
   - Automated backup and point-in-time recovery

## Architecture Diagrams

### Diagram 1: AWS Database Services Overview

```mermaid
graph TB
    A[AWS Database Services] --> B[Relational Databases]
    A --> C[NoSQL Databases]
    A --> D[Data Warehousing]
    A --> E[In-Memory Databases]
    A --> F[Graph Databases]
    A --> G[Time Series Databases]
    A --> H[Ledger Databases]
    
    B --> B1[Amazon RDS<br/>Managed SQL]
    B --> B2[Amazon Aurora<br/>High Performance]
    B --> B3[RDS on EC2<br/>Custom Control]
    
    C --> C1[Amazon DynamoDB<br/>Key-Value & Document]
    C --> C2[Amazon DocumentDB<br/>MongoDB Compatible]
    
    D --> D1[Amazon Redshift<br/>Data Warehousing]
    D --> D2[Amazon EMR<br/>Big Data Processing]
    
    E --> E1[Amazon ElastiCache<br/>Redis & Memcached]
    
    F --> F1[Amazon Neptune<br/>Graph Database]
    
    G --> G1[Amazon Timestream<br/>Time Series]
    
    H --> H1[Amazon QLDB<br/>Ledger Database]
