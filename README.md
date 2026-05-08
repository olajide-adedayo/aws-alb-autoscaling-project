# AWS ALB + Auto Scaling Group (ASG) Project

## 📌 Project Overview

This project demonstrates the design and deployment of a highly available and scalable web infrastructure on AWS using Application Load Balancer (ALB) and Auto Scaling Group (ASG).

It simulates a real-world production environment where traffic is distributed across multiple servers, and new instances are automatically launched based on demand.

---

## 🧠 Architecture

```text
User
  ↓
Application Load Balancer (ALB)
  ↓
Target Group
  ↓
EC2 Instances (Apache Web Servers)
  ↓
Auto Scaling Group (ASG)

##   AWS Services Used

Amazon EC2 (Elastic Compute Cloud)
Application Load Balancer (ALB)
Target Groups
Auto Scaling Group (ASG)
Launch Template
Security Groups
Elastic Load Balancing Health Checks
Apache HTTP Server

##  Project Implementation

###  1. EC2 Instance Setup
Launched multiple EC2 instances
Installed Apache HTTP Server
Configured simple web pages for identification (Server 1 & Server 2)

###  2. Application Load Balancer (ALB)
Created ALB to distribute incoming traffic
Configured listener on HTTP port 80
Linked ALB to target group

###  3. Target Group Configuration
Registered EC2 instances as targets
Configured health checks using HTTP (port 80)
Verified all instances as healthy and serving traffic

###  4. Auto Scaling Group (ASG)
Created Launch Template for EC2 configuration
Configured Auto Scaling Group
Enabled ELB health checks
Set minimum, desired, and maximum capacity
Automatically launched additional EC2 instances when needed

##  ✅ Validation & Testing
Verified ALB DNS endpoint in browser
Confirmed traffic distribution across multiple EC2 instances
Observed switching between:
Server 1 (EC2 Instance)
Server 2 (EC2 Instance)
Auto Scaling instances
Confirmed all targets in Target Group were healthy
Validated Auto Scaling functionality

## 📸 Screenshots

### ALB Working in Browser
![ALB Working](screenshots/alb-working-browser.png)

---

### Server 1 (EC2 Instance)
![Server 1](screenshots/server-1-apache-54-81-207-157.png)

---

### Server 2 (EC2 Instance)
![Server 2](screenshots/server-2-apache-18-209-175-8.png)

---

### Target Group Health Status
![Target Group](screenshots/alb-target-group-4-healthy.png)


##  🎯 Key Outcomes
Built a highly available AWS architecture
Implemented load balancing across multiple EC2 instances
Configured automatic scaling based on demand
Gained hands-on experience with AWS networking and compute services
Understood health checks and fault tolerance mechanisms


##  📚 Skills Demonstrated
AWS EC2
Application Load Balancer (ALB)
Auto Scaling Group (ASG)
Target Groups & Health Checks
AWS Security Groups
Apache Web Server Deployment
Cloud Architecture Design
High Availability Systems


##  👨‍💻 Author
Olajide Adedayo
