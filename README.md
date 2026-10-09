AWS Application Load Balancer, Auto Scaling & KMS

Hands-on AWS Infrastructure Lab | Cloud Computing & DevOps

📌 Project Overview

This project documents the configuration of AWS infrastructure components for load balancing, EC2 instance scaling, and encryption key management.

The lab covers an internet-facing Application Load Balancer (ALB), target groups, EC2 launch templates, an Auto Scaling Group (ASG), security groups, and AWS Key Management Service (KMS).

The objective was to gain practical familiarity with AWS compute, networking, scalability, and security services.

🎯 Objectives

- Configure an Application Load Balancer to handle incoming application traffic.
- Create a target group for registering application instances.
- Configure an EC2 launch template for instance provisioning.
- Create an Auto Scaling Group with configurable capacity.
- Configure security groups for network access control.
- Create a customer-managed KMS key for learning AWS key management.

🛠️ AWS Services Used

Service| Purpose
Amazon EC2| Compute instances for application hosting
Application Load Balancer (ALB)| Distributes incoming HTTP/HTTPS traffic across registered targets
EC2 Auto Scaling| Manages the number of EC2 instances according to group settings and scaling policies
EC2 Launch Templates| Defines instance launch configuration
Target Groups| Registers targets and performs health checks
Amazon VPC & Security Groups| Provides network isolation and access control
AWS Key Management Service (KMS)| Manages encryption keys

🏗️ Implementation

1. Application Load Balancer

- Created an internet-facing Application Load Balancer.
- Configured a target group for application targets.
- Configured a security group for network access.

2. EC2 Launch Template

- Created a launch template to define the configuration used when launching EC2 instances.
- Used the launch template as part of the Auto Scaling setup.

3. Auto Scaling Group

- Created an EC2 Auto Scaling Group named "mobile-ASG".
- Configured the group's minimum, desired, and maximum capacity settings.
- Connected the Auto Scaling configuration with the load-balancing setup.

4. AWS KMS

- Created a customer-managed KMS key named "ec2-kms-key".
- Practiced the AWS KMS key-management workflow.

Note: Creating a KMS key alone does not demonstrate that data or an EC2 volume was encrypted using that key.

🧪 Validation & Evidence

The repository includes screenshots documenting the AWS resource configuration.

The following tests can be performed to validate the end-to-end behavior:

- Verify that the ALB DNS endpoint serves the application.
- Confirm that the target group reports healthy registered targets.
- Terminate an instance and verify that the Auto Scaling Group replaces it.
- Trigger a configured scaling policy and observe the resulting capacity change.
- Verify encryption using the KMS key if an encryption use case is implemented.

These tests should be marked as completed only after their results have been verified.

📚 Key Learning Outcomes

- Understanding the relationship between load balancers, target groups, launch templates, and Auto Scaling Groups.
- Learning how EC2 capacity can be managed through Auto Scaling configuration.
- Understanding the role of security groups in controlling network traffic.
- Gaining introductory experience with AWS KMS and customer-managed keys.
- Practicing AWS resource configuration through the AWS Management Console.

📸 Screenshots

See the project PDF and accompanying screenshots in this repository for evidence of the configuration steps.

💰 Cost Management

AWS resources used in this lab may incur charges, including the Application Load Balancer, EC2 instances, public IPv4 addresses, and KMS key storage.

- Review current AWS pricing before deploying resources.
- Delete resources when testing is complete.
- Remove unused load balancers, Auto Scaling Groups, EC2 instances, and associated resources.
- Review KMS key deletion requirements before scheduling deletion.

👨‍💻 Author

Akash K

- GitHub: "Akash-k1" (https://github.com/Akash-k1)

Focus Areas: AWS Cloud, Cloud Support, DevOps, Infrastructure Management
