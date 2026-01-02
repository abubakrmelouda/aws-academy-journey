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
   - Integrated Triggers: Works with more than 200 AWS services as event sources

3. **Containers & Platform Services:**
   - Containers vs VMs: Lightweight, portable application packages that share the host OS kernel
   - Amazon ECS/EKS: Managed container orchestration services
   - AWS Fargate: Serverless compute engine for containers
   - AWS Elastic Beanstalk: Platform-as-a-Service (PaaS) for easy web application deployment

## Module Completion Evidence
- 8 instructional videos + EC2 console demonstration completed
- Reviewed comprehensive Learner Guide
- **Completed Lab 3: Introduction to Amazon EC2**
- **Completed AWS Lambda Activity**
- **Completed AWS Elastic Beanstalk Activity**
- **Achieved 100% on Knowledge Check**
- Explored EC2, Lambda, and Elastic Beanstalk consoles

## Hands-On Lab: Introduction to Amazon EC2

### **Lab Objectives Achieved:**
1. **Created and Configured EC2 Instance:**
   - Successfully launched Amazon Linux 2 instance using console wizard
   - Selected appropriate t2.micro instance type
   - Configured key pair for secure SSH access
   - Set up security group with proper inbound rules

2. **Managed Instance Lifecycle:**
   - Successfully retrieved system logs via console for troubleshooting
   - Updated security group to add new inbound rules
   - Modified instance attributes (changed instance type)
   - Properly stopped instance using correct procedure

3. **Troubleshooting and Monitoring:**
   - Learned that instances must be stopped before modifying certain attributes
   - Understood the difference between stop and terminate actions
   - Practiced monitoring instance status and health checks
   - Retrieved and analyzed system logs for debugging

### **Lab Performance:**
- **Task 1:** EC2 instance created correctly
- **Task 2:** System log requested successfully
- **Task 3:** Security group updated correctly
- **Task 4:** EC2 instance updated successfully
- **Task 6:** Instance stopped on second attempt

### **Key Learnings from EC2 Lab:**
1. **Instance Creation Process:**
   - Importance of selecting the right AMI for your workload
   - Proper key pair management for secure access
   - Security group configuration for network security

2. **Instance Management:**
   - Instance lifecycle states (pending, running, stopping, stopped, terminated)
   - System logs as a troubleshooting tool
   - Instance modification requirements and limitations

3. **Best Practices Discovered:**
   - Always stop instances before modifying attributes like instance type
   - Use security groups to implement least privilege network access
   - Monitor instance metrics for performance optimization

## Hands-On Activity: AWS Lambda

### **Activity Objectives:**
1. **Created Lambda Function:**
   - Built Lambda function to stop EC2 instances on schedule
   - Configured Python 3.8 runtime environment
   - Set up IAM execution role with EC2 permissions

2. **Configured Event Bridge Rules:**
   - Created scheduled expression execution
   - Set up CloudWatch Events rule to trigger Lambda function
   - Configured event pattern matching

3. **Serverless Architecture Implementation:**
   - Understood event-driven execution model
   - Implemented serverless cost optimization strategy
   - Automated infrastructure management

### **Activity Performance:**
- **Task 1:** Lambda function created
- **Task 2:** Scheduled expression configured
- **Task 3:** Lambda function configured
- **Task 4:** Instance stopped

### **Challenges and Solutions:**
- **Challenge:** Lambda function failed to stop EC2 instances due to IAM permission issues
- **Solution:** Created dedicated IAM role with `ec2:StopInstances` and `ec2:DescribeInstances` permissions
- **Learning:** IAM role configuration is critical for Lambda function execution

## Hands-On Activity: AWS Elastic Beanstalk

### **Activity Objectives:**
1. **Deployed Web Application:**
   - Accessed Elastic Beanstalk console successfully
   - Deployed sample web application with perfect score
   - Understood automatic infrastructure provisioning

2. **Infrastructure Management:**
   - Verified EC2 instances created by Elastic Beanstalk
   - Observed automatic load balancer configuration
   - Monitored application health dashboard

3. **PaaS Benefits Realized:**
   - Faster deployment compared to manual EC2 setup
   - Automatic scaling and load balancing configuration
   - Focus on application code rather than infrastructure

### **Activity Performance:**
- **Task 1:** Beanstalk console accessed
- **Task 2:** App deployed
- **Task 3:** EC2 console accessed

### **Key Benefits Observed:**
1. **Rapid Deployment:** Application deployed in minutes vs hours of manual setup
2. **Managed Infrastructure:** AWS handles OS updates, security patches and scaling
3. **Developer Productivity:** Focus on code not infrastructure management

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
