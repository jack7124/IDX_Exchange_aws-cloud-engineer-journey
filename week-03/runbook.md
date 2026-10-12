# Week 03 write up
### Concepts: AMIs, instance types (t3.micro = Free Tier), security groups (stateful, instance-level) vs NACLs
### (stateless, subnet-level), EBS volumes, user data bootstrapping.


##### This week, I tackled AWC EC2 Instance compute and clean up, alongside with security practices.

In Week 3, we launched an EC2 instance using the Amazon Linux 2023 AMI, which provided the operating-system image for the server. We selected a t3.micro instance type because PropertyLite is a lightweight application that does not require significant compute resources. We configured an instance-level security group to control inbound traffic, allowing SSH on port 22 from my local IP and allowing TCP traffic on port 8080 for the Flask application. We also used EC2 user data as a bootstrap script so the instance could automatically install dependencies, create the PropertyLite application files, and start the Flask server at launch. Finally, I secured the SSH private key using chmod 400 and verified the application by using curl against both localhost:8080 from the EC2 instance and the instance's public IP from my local machine.
