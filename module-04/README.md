# Module 4: AWS Cloud Security

**Completed:** October 21, 2025  
**Knowledge Check:** 90/100  
**Lab Score:** 40/40 (100%) 
**Time Spent:** 120 minutes

## 3 Key Concepts:

1. **AWS Shared Responsibility Model:**
   - **AWS Responsibility (Security OF the Cloud):** Physical infrastructure, hardware, facilities, network infrastructure, virtualization layer
   - **Customer Responsibility (Security IN the Cloud):** Data encryption (at rest & in transit), network configuration, IAM management, operating system security, application security
   - **Service Model Impact:** IaaS (more customer responsibility) PaaS and SaaS (more AWS responsibility)

2. **AWS Identity and Access Management (IAM):**
   - **Users:** People with credentials (password + access keys)
   - **Groups:** Collections of users with shared permissions
   - **Roles:** Temporary credentials for AWS services or cross-account access
   - **Policies:** JSON documents defining permissions (Allow/Deny)
   - **Principle of Least Privilege:** Grant minimal permissions needed

3. **Security Best Practices & Tools:**
   - **Root Account Protection:** Enable MFA, create IAM admin users
   - **Data Encryption:** AWS KMS for key management, TLS for data in transit
   - **Compliance Tools:** AWS Config, AWS Artifact, CloudTrail logging
   - **DDoS Protection:** AWS Shield (Standard free, Advanced paid)

## Module Completion Evidence
- 6 instructional videos + console demo completed
- Reviewed learner Guide
- **Completed Lab: Introduction to AWS IAM (40/40 - 100%)**
- **Achieved 90% on Knowledge Check**
- Explored IAM console and security configurations

## Hands-On Lab: Introduction to AWS IAM

### **Lab Objectives Achieved:**
1. **Created IAM Users & Groups:**
   - User-1 → S3-Support group (S3 read-only access)
   - User-2 → EC2-Support group (EC2 describe/start/stop)
   - User-3 → EC2-Admin group (Full EC2 access)

2. **Tested Permission Boundaries:**
   - User-2: Could access EC2 Instance but not S3.

3. **Validated Security Principle:**
   - **Principle of Least Privilege** demonstrated
   - **Explicit Deny overrides Allow** verified
   - **Group-based permission management** implemented

### **Lab Architecture:**

<img width="1380" height="718" alt="image" src="https://github.com/user-attachments/assets/ebdfc88a-c9ad-4436-840d-7a689c69e817" />
