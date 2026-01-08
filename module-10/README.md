# Module 10: Auto Scaling and Monitoring.

**Completed:** January 6, 2026  
**Knowledge Check:** (90%)  
**Lab Score:** 30/35 (86%)  
**Time Spent:** 8 hours

## Overview
Module 10 focuses on building scalable and resilient architectures using AWS Auto Scaling, Load Balancing, and Monitoring services. This module teaches how to create architectures that automatically adjust to demand while maintaining high availability.

## Key Concepts

### 1. Elastic Load Balancing (ELB)
AWS service that distributes incoming application or network traffic across multiple targets (EC2 instances, containers, IP addresses, Lambda functions) across single or multiple Availability Zones.

#### Types of Load Balancers:
- **Application Load Balancer (ALB):** Layer 7, HTTP/HTTPS traffic, content-based routing
- **Network Load Balancer (NLB):** Layer 4, TCP/UDP traffic, ultra-low latency
- **Classic Load Balancer (CLB):** Legacy, both Layer 4 and 7

#### Key Features:
- **Health Checks:** Monitors target health, stops routing to unhealthy targets
- **Listeners:** Configured with protocol and port for incoming traffic
- **Target Groups:** Groups of registered targets for ALB and NLB
- **High Availability:** Distributes traffic across multiple AZs

### 2. Amazon CloudWatch
Monitoring and observability service that collects and tracks metrics, monitors log files, sets alarms, and automatically reacts to changes in AWS resources.

#### Key Components:
- **Metrics:** Variables you can measure (CPU utilization, request latency, etc.)
- **Alarms:** Monitor metrics and trigger actions (SNS notifications, Auto Scaling actions)
- **Events:** React to operational changes in real-time
- **Logs:** Collect, monitor, and store log files

#### Alarm Configuration:
- **Static Threshold:** Breach-based alarms
- **Anomaly Detection:** ML-based pattern recognition
- **Metric Math:** Mathematical operations on metrics

### 3. Amazon EC2 Auto Scaling
Service that helps maintain application availability by automatically adding or removing EC2 instances based on defined conditions.

#### Auto Scaling Group Components:
- **Minimum Size:** Minimum number of running instances
- **Desired Capacity:** Target number of instances
- **Maximum Size:** Maximum number of instances
- **Scaling Policies:** Rules for when to scale in/out
- **Launch Configuration/Template:** Instance configuration template

#### Scaling Methods:
1. **Manual Scaling:** Adjust capacity manually
2. **Scheduled Scaling:** Based on date/time patterns
3. **Dynamic Scaling:** Based on CloudWatch metrics (CPU utilization, etc.)
4. **Predictive Scaling:** ML-based forecasting (AWS Auto Scaling)

#### Scaling Actions:
- **Scale Out:** Launch new instances
- **Scale In:** Terminate instances
- **Health Checks:** Replace unhealthy instances automatically

### 4. Integrated Architecture Pattern
ELB, Auto Scaling, CloudWatch offers Dynamic, Scalable Infrastructure

**Flow:**
1. CloudWatch monitors metrics (CPU utilization, request count)
2. When threshold breached → CloudWatch alarm triggers
3. Auto Scaling policy executes → Scale in/out
4. ELB automatically registers new instances
5. Traffic distributed across healthy instances

## Module Completion

### Achievements:
- Completed all instructional videos on ELB, CloudWatch, and Auto Scaling
- Reviewed comprehensive learner guide materials
- **Completed Lab 6: Scale & Load Balance Architecture**
- **Achieved 90% on Knowledge Check (45/50)**
- Explored AWS Management Console for all three services
- Practiced integrated architecture design patterns

## Hands-On Lab: Scale & Load Balance Architecture

### Lab Objectives Achieved:
1. **Created AMI from Running Instance:**
   - Successfully created Amazon Machine Image from existing web server
   - Configured appropriate naming and tagging

2. **Built Application Load Balancer:**
   - Created Autoscale Load Balancer with listener configuration (HTTP:80)
   - Configured target groups and health checks
   - Set up security groups for ALB access

3. **Configured Auto Scaling:**
   - Created Launch Template with AMI, instance type, security groups
   - Configured Auto Scaling Group with min/desired/max capacity
   - Set up scaling policies based on CPU utilization

4. **Integrated Architecture:**
   - Connected ALB to Auto Scaling Group
   - Verified automatic instance registration
   - Tested load balancing across multiple instances

5. **Monitoring Setup:**
   - Created CloudWatch alarms for CPU utilization
   - Configured SNS notifications for scaling events
   - Monitored infrastructure performance

### Lab Performance:
**Total Score:** 30/35 (86%)

**Task Breakdown:**
- Task 1: AMI created
- Task 2: Load Balancer created
- Task 3a: Launch Template created
- Task 3b: Auto Scaling Group created
- Task 4: Load Balancer verified
- Task 5: Auto Scaling verified
- Task 6: Web Server 1 verified

## Key Takeaways

### Technical Competencies:
1. **Architectural Design:** Created integrated scaling solutions
2. **Load Balancing:** Configured ALB with target groups and health checks
3. **Auto Scaling:** Implemented dynamic scaling policies
4. **Monitoring:** Set up comprehensive CloudWatch monitoring
5. **Troubleshooting:** Debugged scaling and load balancing issues

### Business Impact:
1. **Cost Optimization:** Pay only for needed capacity
2. **High Availability:** Maintain service during instance failures
3. **Performance:** Ensure consistent application performance
4. **Operational Excellence:** Reduced manual intervention
   
### Architecture Built:
