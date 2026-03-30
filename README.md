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
