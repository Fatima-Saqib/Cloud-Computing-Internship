# Project 2 - The Server Commander

## Overview
This project demonstrates how to provision and configure a Linux virtual machine on AWS using Amazon EC2. The server was accessed securely using SSH, Apache Web Server was installed, and a custom webpage was hosted successfully.

## Objective
- Launch an Ubuntu EC2 instance.
- Connect to the server using SSH.
- Install and configure the Apache web server.
- Host a custom webpage displaying **"Welcome to DecodeLabs"**.

## AWS Services Used
- Amazon EC2
- Security Groups
- SSH
- Ubuntu Server 24.04 LTS
- Apache2

## Steps Performed
1. Launched an Ubuntu EC2 instance.
2. Configured Security Group rules for SSH (Port 22) and HTTP (Port 80).
3. Connected to the instance using SSH from PowerShell.
4. Updated the system packages.
5. Installed Apache Web Server.
6. Started and enabled the Apache service.
7. Replaced the default webpage with a custom HTML page.
8. Verified the webpage through the EC2 Public IPv4 address.

## Commands Used

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
echo "<h1>Welcome to DecodeLabs</h1>" | sudo tee /var/www/html/index.html
```

## Output
The web server successfully displayed the following webpage:

**Welcome to DecodeLabs**

## Project Status
✅ Completed
