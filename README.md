# E-12-LAB-EC2-AMI-Backup-Restore-
This project demonstrates how to create an Amazon EC2 instance, configure a web server, generate an Amazon Machine Image (AMI) as a backup, and launch a new instance from that AMI.


# 🎯 Objectives
Launch EC2 instance (t2.micro)
Install and configure Apache (httpd)
Create sample files
Create AMI (backup of instance)
Launch a new EC2 instance from AMI
Verify data and configuration persistence

# 🏗️ Architecture
```bash

EC2 (t2.micro)
   │
   ├── Apache Installed
   ├── Test Files Created
   │
   ▼
AMI (Backup Image)
   │
   ▼
EC2 (t3.micro from AMI)


```

# ⚙️ Prerequisites
AWS Account
Key Pair (ssh22.pem)
Basic knowledge of SSH

# Step 1: Launch EC2 Instance

- Name: web-server-1
- AMI: Amazon Linux 2
-  Instance Type: t2.micro
-  Key Pair: ssh22
-  Security Group: Allow SSH (22) and HTTP (80)

# Step 2: Connect to EC2

```bash 
ssh -i ssh22.pem ec2-user@<Public-IP>

```

```bash

sudo su

```
# Step 3: Install Apache Web Server
```bash
yum install httpd -y
```

```bash
sysystemctl start httpd
```


```bash
systemctl start httpd
```

```bash
systemctl enable httpd
```









