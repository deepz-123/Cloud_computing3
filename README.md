# Cloud_computing3
**COMPANY**      : CODTECH IT SOLUTIONS
**NAME**         : DEEPAK 
**INTERN ID**    : CT04MRV
**DOMAIN**       : CLOUD COMPUTING 
**DURATION **    : 4 MONTHS 
**MENTOR**       : NEELA SANTOSH 
**DESCRIPTION**  :

**Task 3: Design a Multi-Cloud Architecture (AWS-Focused)**

This project demonstrates the design and simulation of a multi-cloud architecture using Amazon Web Services (AWS), with provisions for future interoperability with another cloud provider (e.g., Azure or GCP). While all configurations are performed within AWS, the architecture is designed to accommodate seamless integration with external cloud platforms.
Key Steps & Features

Step 1: VPC Creation

A VPC named MultiCloud-VPC is created with a CIDR block of 10.0.0.0/16.

Two public subnets (10.0.1.0/24 and 10.0.2.0/24) are configured across two availability zones.

An Internet Gateway (MultiCloud-IGW) is attached and route tables are updated for external traffic.


Step 2: EC2 Instance Launch

A Linux-based EC2 instance (MultiCloud-WebServer) is deployed in the public subnet.

Apache, PHP, and MySQL client are installed to host a basic web application.

Security Groups (WebServer-SG) are configured to allow HTTP, HTTPS, and SSH access.


Step 3: RDS MySQL Setup

A MySQL RDS instance (multicloud-db) is deployed using the free tier.

The database is placed in the public subnet for demo purposes.

A PHP script is added to the EC2 instance to test connectivity with the RDS instance.


Step 4: IAM Role Configuration

An IAM Role (EC2-S3-Access) is created with the AmazonS3FullAccess policy.

This role is attached to the EC2 instance to simulate cross-cloud data access.


Step 5: Sample Web App Deployment

A PHP-based web page (index.php) connects to the RDS database.

Successful database connection is confirmed via browser output: "Connected to RDS successfully!"


Step 6: Simulated Cross-Cloud via S3

An S3 bucket (multicloud-demo-bucket) is created.

The EC2 instance uploads a file (test.txt) to S3 using AWS CLI.

This demonstrates how data can be shared with external services/clouds.


Step 7: Architecture Documentation

A visual architecture diagram is created using AWS Architecture Icons or draw.io.

It shows the interaction between EC2, RDS, S3, and a placeholder for an external cloud provider.

The diagram is accompanied by a brief explanation of how data flows across components.
