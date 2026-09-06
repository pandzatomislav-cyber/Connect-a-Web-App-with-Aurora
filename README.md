<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Connect a Web App with Aurora

**Project Link:** [View Project](http://nextwork.ai/projects/aws-databases-webapp)

**Author:** Tomislav Pandza  
**Email:** pandza.tomislav@gmail.com

---

## Connect a Web App to Amazon Aurora

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-databases-webapp_1709b26b)

---

## Introducing Today's Project!

### What is Amazon Aurora?

AWS Aurora is a type of relational database. We'd use AWS Aurora if we needed something large-scale, with peak performance and uptime. This is because Aurora databases use clusters. Ordinary relational databases, like MySQL and Oracle are more generic and cost-effective. They suit smaller databases and less demanding workloads.

### How I used Amazon Aurora in this project

In today's project, I used Amazon Aurora to:
1.  Create an Aurora MySQL Database
2. Launch and Configure an EC2 Instance
3. Build and Connect a Web Application
4.  Test and Verify Database Interactions

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was that you can use sql in the CLI. Something new to learn everyday I guess!

### This project took me...

This project took me about 2 hours in total.

---

## Creating a Web App

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-databases-webapp_b7999168)

To connect to my EC2 instance, I had to access my terminal and go into PowerShell using the pwsh command. This way I could navigate my desktop with ease. I double checked if my pem file was there. After that I put in the command to access the VM I created thorugh the terminal and it was a success.

To help me create my web app, I first had to update the software with ''sudo dnf update -y'', then with ''sudo dnf install -y httpd php php-mysqli mariadb105'' I installed the Apache web server, then PHP, php-mysqli and Maria DB. Finally, with "sudo systemctl start httpd", I started the most basic verison of my web app.

---

## Connecting my Web App to Aurora

I set up my EC2 instance's connection details to my database by first giving permission to the EC2 user instead of the root user, I created a new sub-folder in the "www" folder called "inc". In that folder I created a file "dbinfo.inc" and adjusted the file in the terminal to have the code to connect my EC2 instance to my Aurora database to the dbinfo.inc file.

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-databases-webapp_1709b25b)

---

## My Web App Upgrade

Next, I upgraded my web app by writing the big block of code in the SamplePage.php file and that's what makes our new web app look so cool! It's pulling in the details from our dbinfo.inc file we created earlier and using it to display up-to-date changes directly from our website

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-databases-webapp_2709b25b)

---

## Testing my Web App

To make sure my web app was working correctly, I had to connect my database with MYSQL CLI.  It provides direct access to all MySQL features, supports automation, and is a preferred method for managing databases on remote servers, such as EC2 instances.

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-databases-webapp_1409z22b)

---

---
