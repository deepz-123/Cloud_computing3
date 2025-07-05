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

**OUTPUT**

**Step 1: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/70e13bc3-e3b1-4a6c-b76c-b0d73e5e5469" />

**Step 2: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/a7fb2d0d-113c-4ff2-8a65-c1c6a5121353" />

**Step 3: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/5a5cfc59-a9db-47da-8308-6641f07d894e" />

**Step 4: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/dd30e70b-49ff-49e2-acc1-6a3b80b7e16c" />

**Step 5** 

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/fd76476b-f64b-4835-b780-a9dc0cd23c00" />

**Step 6: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0f0c0c6c-3756-41a3-8237-7503a34178b7" />

**Step 7**

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0d590f32-100c-4929-9d76-c4e217a21b27" />

**Step 8: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/7a61c55a-0e30-4f7d-8d14-52d3c0434a51" />

**Step 9: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/debd0b89-290c-47ba-aeaa-d63ed41ef566" />

**Step 10: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/6373067a-0cb1-442e-9b1f-7a1423c20ba2" />

**Step 11: **

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0c98e0e5-7c23-4783-8177-81ab04c2f04e" />
