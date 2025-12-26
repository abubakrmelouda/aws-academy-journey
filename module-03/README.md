# Module 3: AWS Global Infrastructure Overview

**Completed:** October 20, 2025  
**Knowledge Check:** 90/100  
**Time Spent:** 75 minutes

## 3 Key Concepts:

1. **AWS Global Infrastructure Hierarchy:**
   - **Regions:** more than 31 geographical areas (e.g. US, EU)
   - **Availability Zones (AZs):** Isolated data centers within regions (more than 3 per region)
   - **Edge Locations:** more than 400 points of presence for CloudFront & Route 53
   - **Data Centers:** Physical facilities where servers reside

2. **Availability Zone Design Principles:**
   - **Fault Isolation:** AZs are physically separated (kilometers apart)
   - **High Availability:** Designed to survive disasters (earthquakes, storms)
   - **Low Latency:** Connected via redundant fiber (<100km apart)
   - **Synchronous Replication:** Data can be replicated between AZs in real-time

3. **AWS Service Categories Overview:**
   - **Compute:** EC2, Lambda, Elastic Beanstalk, ECS, EKS
   - **Storage:** S3, EBS, EFS, S3 Glacier
   - **Database:** RDS, DynamoDB, Aurora, Redshift
   - **Networking:** VPC, CloudFront, Route 53, ELB
   - **Security:** IAM, Organizations, KMS, Shield
   - **Management:** CloudWatch, CloudTrail, Trusted Advisor

## Module Completion:
- 3 instructional videos completed
- Learner Guide reviewed
- **Achieved 90% on Knowledge Check**
- Explored AWS Management Console
- Understood service categorisation

## Key Insights from the module:

### **Region Selection Factors:**
1. **Data Governance:** Legal requirements (e.g., EU data must stay in EU)
2. **Latency:** Proximity to users (use Cloud Ping to test)
3. **Service Availability:** Not all services available in all regions
4. **Cost Variation:** Pricing differs by region
5. **Compliance:** Specific regions for specific needs (AWS GovCloud in Asia)

### **Availability Zone Characteristics:**
- Each AZ has **multiple data centers** (typically 3)
- Fully isolated with **independent power and networking**
- **100km maximum distance** between AZs in same region
- **High-bandwidth, low-latency connections** between AZs
- Customers must **manually select and replicate** across AZs

### **Edge Locations vs Regional Edge Caches:**
| Feature | Edge Locations | Regional Edge Caches |
|---------|----------------|----------------------|
| **Purpose** | Frequent content delivery | Less frequent content |
| **Latency** | Lowest possible | Higher than edge |
| **Use Case** | Hot content | Warm content |
| **Services** | CloudFront, Route 53 | CloudFront |

## Real-World Application
As a **Cloud Architect**, I understand how to:

1. **Design multi-AZ architectures** for high availability applications
2. **Select optimal regions** based on compliance, latency, and cost
3. **Implement CloudFront** with edge locations for global low-latency delivery
4. **Plan disaster recovery** using cross-region replication strategies
5. **Navigate AWS service catalog** by understanding category organization

## Key Resources from Module 3
- [AWS Global Infrastructure Map](https://aws.amazon.com/about-aws/global-infrastructure/)
- [AWS Region Table](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/)
- [Cloud Ping Test](https://www.cloudping.info/)
- [AWS Service Catalog](https://aws.amazon.com/products/)

**Previous:** [Module 2: Cloud Economics ←](../module-02/README.md)  
**Next:** [Module 4: AWS Cloud Security →](../module-04/README.md)

*"AWS's global infrastructure provides the foundation for resilient, scalable, and performant cloud solutions."*
