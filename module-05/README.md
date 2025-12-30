# Module 5: Networking and Content Delivery

**Completed:** October 22, 2025  
**Knowledge Check:** 90/100  
**Lab Score:** 25/30 (83%)  
**Time Spent:** 120 minutes

## 3 Key Concepts:

1. **Amazon Virtual Private Cloud (VPC) Fundamentals:**
   - **VPC:** Logically isolated network section in AWS (your private cloud slice)
   - **Subnets:** Segments of VPC in specific Availability Zones (public/private)
   - **CIDR Blocks:** IP address ranges (e.g., 10.0.0.0/16 = 65,536 addresses)
   - **Route Tables:** Direct traffic between subnets and gateways
   - **Internet Gateway (IGW):** Connects VPC to public Internet

2. **VPC Security & Networking Components:**
   - **Security Groups:** Instance-level firewall (stateful, allow rules only)
   - **Network ACLs:** Subnet-level firewall (stateless, allow/deny rules)
   - **NAT Gateway:** Allows private subnet instances to access Internet
   - **Elastic IP:** Static public IPv4 address
   - **VPC Peering:** Connect two VPCs privately

3. **Content Delivery & DNS Services:**
   - **Amazon Route 53:** DNS service with routing policies (latency, geolocation, failover)
   - **Amazon CloudFront:** Content Delivery Network (CDN) with edge locations
   - **DNS Resolution:** Translates domain names to IP addresses

## Module Completion Evidence
-  6 instructional videos + VPC wizard console completed
- Reviewed learner Guide
- **Completed Lab: Build VPC and Launch Web Server (25/30)**
- **Achieved 90% on Knowledge Check**
- Explored VPC console and networking configurations

## Hands-On Lab: Build VPC and Launch Web Server

### **Lab Objectives Achieved:**
1. **Created Custom VPC:**
   - VPC with CIDR block configuration
   - Public and private subnets in different AZs
   - Internet Gateway attached to VPC

2. **Configured Networking Components:**
   - Route tables with proper routes (0.0.0.0/0 to IGW)
   - Security group allowing HTTP/SSH access
   - EC2 instance launched in public subnet

3. **Launched Web Server:**
   - EC2 instance with web server software
   - Website accessible via public IP
   - Network connectivity verified

### **Lab Performance:**
**Score:** 25/30 (83%)
- **Task 1:** VPC created correctly (5/5)
- **Task 2:** New subnets created correctly (5/5)
- **Task 3:** Security group created correctly (5/5)
- **Task 4a:** EC2 instance created correctly (5/5)
- **Task 4b:** EC2 instance website accessible (5/5)
