# 🏗️ VPC Architecture using AWS

## 📖 Overview
This project demonstrates the design and implementation of a **Virtual Private Cloud (VPC)** architecture in **Amazon Web Services (AWS)**.  
It showcases how to create a secure, scalable, and highly available network infrastructure for deploying applications and services.

---

## 🧩 Architecture Components

### 1. **VPC**
- Custom VPC with a defined CIDR block (e.g., `10.0.0.0/16`)
- Enables secure communication within AWS resources

### 2. **Subnets**
- **Public Subnets** – For resources like Load Balancers and Bastion Hosts  
- **Private Subnets** – For Application and Database servers  
- Located in **multiple Availability Zones (AZs)** for high availability

### 3. **Internet Gateway (IGW)**
- Allows outbound internet access for public resources

### 4. **NAT Gateway**
- Enables instances in private subnets to access the internet securely (e.g., for updates)

### 5. **Route Tables**
- Separate route tables for public and private subnets  
- Configured with appropriate routes to control traffic flow

### 6. **Security Groups & NACLs**
- **Security Groups:** Instance-level firewalls  
- **Network ACLs:** Subnet-level firewalls for extra security layers

### 7. **Bastion Host**
- Deployed in the public subnet for secure SSH access to private instances

### 8. **Application & Database Layers**
- Application servers in private subnets  
- Database servers (RDS or EC2) in isolated subnets with no public access

---

## 🧠 Key Features
- ✅ Highly available network design across multiple AZs  
- 🔒 Secure architecture using layered security (Security Groups + NACLs)  
- 🌐 Controlled internet access via NAT and IGW  
- ⚙️ Scalable and modular setup suitable for enterprise-grade deployments  

---

## 🗺️ Architecture Diagram
*(Insert your diagram here)*  
Example:
