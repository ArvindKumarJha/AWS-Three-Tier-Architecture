# AWS Three-Tier Architecture

## 📌 Project Overview

This project demonstrates the implementation of a highly available, scalable, and secure Three-Tier Architecture on Amazon Web Services (AWS). The architecture follows cloud best practices by separating the application into Presentation, Application, and Database tiers while utilizing AWS managed services for improved reliability and performance.

The project is designed to showcase practical cloud architecture skills, networking concepts, security implementation, load balancing, auto scaling, and database management.

---

## 🏗️ Architecture

The application is divided into three logical layers:

### 1. Presentation Tier (Web Tier)
Responsible for receiving user requests and serving web content.

AWS Services Used
- Amazon VPC
- Public Subnets
- Internet Gateway
- Application Load Balancer (ALB)
- EC2 Instances
- Auto Scaling Group
- Security Groups

---

### 2. Application Tier (Business Logic)

Processes application requests received from the web tier.

AWS Services Used
- Private Subnets
- EC2 Instances
- Auto Scaling Group
- Internal Security Groups

---

### 3. Database Tier

Stores application data securely in private subnets.

AWS Services Used
- Amazon RDS (MySQL/PostgreSQL)
- Multi-AZ Deployment
- DB Subnet Group
- Security Groups

---

## 🚀 Features

- Highly Available Architecture
- Multi-AZ Deployment
- Auto Scaling
- Load Balancing
- Secure Networking
- Public and Private Subnets
- Security Groups
- Internet Gateway
- NAT Gateway
- Amazon RDS
- Least Privilege Access
- Scalable Infrastructure
- Fault Tolerant Design

---

## 🛠 AWS Services Used

| Service | Purpose |
|----------|----------|
| Amazon VPC | Network Isolation |
| Public Subnets | Internet-facing resources |
| Private Subnets | Application and Database |
| Internet Gateway | Internet Connectivity |
| NAT Gateway | Outbound Internet Access |
| Route Tables | Traffic Routing |
| EC2 | Compute Instances |
| Application Load Balancer | Traffic Distribution |
| Auto Scaling Group | Automatic Scaling |
| Amazon RDS | Managed Database |
| Security Groups | Instance Firewall |
| IAM | Access Management |
| CloudWatch | Monitoring |
| CloudTrail | Auditing |

---

## 🔐 Security Best Practices

- Resources deployed inside a custom VPC
- Database hosted in private subnet
- Security Groups configured with least privilege
- IAM roles used instead of hardcoded credentials
- Application servers inaccessible from the internet
- Database accessible only from application servers
- NAT Gateway for secure outbound internet access

---

## 📈 High Availability

- Multiple Availability Zones
- Application Load Balancer
- Auto Scaling Groups
- Multi-AZ RDS Deployment
- Health Checks
- Automatic Failover

---

## 🔄 Request Flow

1. User sends request.
2. Request reaches the Application Load Balancer.
3. ALB forwards traffic to Web Tier EC2 instances.
4. Web Tier communicates with Application Tier.
5. Application Tier processes business logic.
6. Application Tier queries Amazon RDS.
7. Database returns requested data.
8. Response is sent back to the user.

---

## 🌐 Network Flow


Internet
     │
     ▼
Application Load Balancer
     │
     ▼
Web Tier (Public Subnets)
     │
     ▼
Application Tier (Private Subnets)
     │
     ▼
Amazon RDS (Private Subnets)


---

## 📊 Benefits

- Improved Security
- Better Scalability
- High Availability
- Fault Tolerance
- Separation of Concerns
- Easy Maintenance
- Cost Optimization
- Production Ready Architecture

---

## 🎯 Learning Outcomes

Through this project, you will understand:

- AWS Networking
- VPC Design
- Public vs Private Subnets
- Route Tables
- NAT Gateway
- Internet Gateway
- Load Balancing
- Auto Scaling
- EC2 Deployment
- Amazon RDS
- IAM Best Practices
- Security Groups
- High Availability Design
- Cloud Architecture Best Practices

---

## 🚀 Deployment Steps

1. Create VPC
2. Create Public and Private Subnets
3. Configure Internet Gateway
4. Configure NAT Gateway
5. Create Route Tables
6. Launch EC2 Instances
7. Configure Application Load Balancer
8. Configure Auto Scaling Groups
9. Create Amazon RDS Instance
10. Configure Security Groups
11. Test End-to-End Connectivity

---

## 👨‍💻 Author

Arvind Kumar Jha

- DevOps Engineer
- AWS Cloud Enthusiast
- Linux & Automation Learner

LinkedIn: https://www.linkedin.com/in/arvind-kumar-jha
