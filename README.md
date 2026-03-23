# AWS EC2 Hands-On Practice

## 👨‍💻 About This Project
This repository demonstrates my hands-on practice with **AWS EC2 (Elastic Compute Cloud)**.  
The project is designed to show step-by-step deployment of a cloud-based virtual server and basic server configuration.

---

## 📌 What is EC2?
Amazon EC2 is a web service that provides resizable compute capacity in the cloud.  
It allows you to launch virtual servers (instances), configure security, and host applications without managing physical hardware.

**Key Features:**
- Scalable compute resources
- Secure network configuration
- Pay-as-you-go pricing
- Multiple instance types (t2.micro, t3.medium, etc.)

---

## ⚙️ Project Objectives
1. Launch a virtual EC2 instance.
2. Connect to the instance using SSH.
3. Configure a basic web server.
4. Document all commands and steps for future reference.

---

## 📝 Steps Performed

### 1. Launch EC2 Instance
1. Log in to the AWS Management Console.
2. Navigate to **EC2 Dashboard**.
3. Click **Launch Instance**.
4. Select **Amazon Linux 2 AMI (Free Tier eligible)**.
5. Choose **t2.micro** instance type.
6. Configure **key pair** (download `.pem` file for SSH access).
7. Configure **security group** to allow **SSH (port 22)** and **HTTP (port 80)**.
8. Launch the instance.

### 2. Connect to EC2 via SSH
```bash
ssh -i my-key.pem ec2-user@<public-ip-address>
3. Install and Start Web Server
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
4. Verify Web Server
Open a browser and enter the EC2 instance public IP.
You should see the default Apache web page.
📷 Screenshots






💡 Lessons Learned
How to launch and manage an EC2 instance.
Basic Linux commands for server management.
How to configure security groups for web access.
Understanding AWS free tier limitations.
🔗 References
AWS EC2 Documentation
Amazon Linux 2 AMI
