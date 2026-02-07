# AWS Static Website Hosting on EC2 🚀

## 📌 Project Overview
In this project, I deployed a static website on an AWS EC2 Linux instance using the Apache HTTP Server.

This project demonstrates hands-on experience with EC2, Linux commands, and web server deployment.

---

## 🛠️ Services & Tools Used
- Amazon EC2
- Security Groups
- Apache HTTP Server (httpd)
- Linux (Amazon Linux)
- GitHub for documentation

---

## ✅ Steps Performed

### 1. Launched an EC2 Instance
- Created an Amazon Linux EC2 server from AWS Console  
- Configured security group to allow:
   - SSH(Port 22)
   - HTTP(Port 80) 

---

### 2. Installed Apache Web Server

```bash
sudo yum update -y
sudo yum install httpd -y

### 3. Started and Enabled Apache Service

```bash
sudo systemctl start httpd
sudo systemctl enable httpd

### 4. Deployed website files

```bash
cd /var/www/html
sudo vi index.html

Uploaded static website content into the Apache web root directory

### 5. Verified website output
http://<EC2-Public-IP>
Accessed the website using the EC2 public IP in a browser
Website was successfully displayed

