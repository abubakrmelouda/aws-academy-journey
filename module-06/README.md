# Module 6: Compute Services

**Completed:** November 1, 2025  
**Knowledge Check:** 100/100  
**Lab Scores:**  
- Lab 3: Introduction to Amazon EC2 - 25/25 (100%)  
- AWS Lambda Activity: 15/20 (75%)  
- AWS Elastic Beanstalk Activity: 25/25 (100%)  
**Time Spent:** 180 minutes

## 3 Key Concepts:

1. **Amazon EC2 - The Foundation of AWS Compute:**
   - Virtual Servers in the Cloud: Provides resizable compute capacity with full control over the OS
   - Instance Types: Optimized for different workloads (General Purpose, Compute Optimized, Memory Optimized, Storage Optimized, Accelerated Computing)
   - Pricing Models: On-Demand, Reserved Instances, Spot Instances, Dedicated Hosts
   - Components: AMIs, Security Groups, Key Pairs, Elastic IPs, EBS Volumes

2. **Serverless Computing with AWS Lambda:**
   - Event-Driven Execution: Run code without provisioning or managing servers
   - Pay-per-Use: Billed only for compute time consumed
   - Automatic Scaling: Scales automatically from a few requests per day to thousands per second
   - Integrated Triggers: Works with 200+ AWS services as event sources

3. **Containerization & Platform Services:**
   - Containers vs VMs: Lightweight, portable application packages that share the host OS kernel
   - Amazon ECS/EKS: Managed container orchestration services
   - AWS Fargate: Serverless compute engine for containers
   - AWS Elastic Beanstalk: Platform-as-a-Service (PaaS) for easy web application deployment

## Module Completion Evidence
- 8 instructional videos + EC2 console demonstration completed
- Reviewed comprehensive Learner Guide
- Completed Lab 3: Introduction to Amazon EC2
- Completed AWS Lambda Activity (15/20)
- Completed AWS Elastic Beanstalk Activity
- Achieved 100% on Knowledge Check
- Explored EC2, Lambda and Elastic Beanstalk consoles

## Architecture Diagrams

### Diagram 1: AWS Compute Services Categories

```mermaid
graph TB
    A[AWS Compute Services] --> B[Infrastructure as a Service]
    A --> C[Serverless Computing]
    A --> D[Container Services]
    A --> E[Platform as a Service]
    
    B --> B1[Amazon EC2<br/>Virtual Machines]
    
    C --> C1[AWS Lambda<br/>Event-driven Functions]
    C --> C2[AWS Fargate<br/>Serverless Containers]
    
    D --> D1[Amazon ECS<br/>Container Orchestration]
    D --> D2[Amazon EKS<br/>Managed Kubernetes]
    D --> D3[Amazon ECR<br/>Container Registry]
    
    E --> E1[AWS Elastic Beanstalk<br/>Web Application Platform]
