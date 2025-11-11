Exercise 1: Launching an Amazon EC2 Instance

This project demonstrates how to **launch, configure, and connect to an Amazon EC2 instance** using the AWS Management Console.  
It was completed as part of my **Cloud Architecture Practicals** for the 5ᵗʰ semester of **BCA (Cloud Computing)** at **Kristu Jayanti College**.

Objective
To understand the steps involved in creating and accessing a virtual server on AWS and to explore key configuration options such as AMI selection, instance type, key pairs, and security groups.

Steps Performed

Log in to AWS Console
- Open the "AWS Management Console" and navigate to "EC2 Service".

Launch a New Instance
- Click "Launch Instance"
- Configure:
  - Name: `MyFirstEC2`
  - AMI: Amazon Linux 2 or Windows Server 2019 Base  
  - Instance Type: `t2.micro (Free Tier eligible)`
  - Key Pair: Create new or select existing for SSH access
  - Storage: 8 GB (default)

Configure Security Group
- Add inbound rules to allow:
  - SSH (22) for Linux connection or RDP (3389) for Windows
  - HTTP (80) if you plan to host a web app

Launch Instance and Connect
- Wait until the instance status shows "running"
- Connect to the instance using:
  - RDP (Windows):
    - Download RDP file and decrypt password using key pair  

Verify Connection
- Successful login confirms instance is up and accessible.  


Result
The EC2 instance was successfully launched and accessed using SSH/RDP.  
Security Group rules and key pair authentication were verified to be functional.


Learning Outcome
- Learned how to launch and connect to an EC2 instance.  
- Understood the role of AMI, Instance Type, Key Pair, and Security Groups.  
- Gained hands-on experience with AWS compute services.
