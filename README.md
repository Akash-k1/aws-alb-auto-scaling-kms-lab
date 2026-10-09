AWS Application Load Balancer, Auto Scaling & KMS

Hands-on AWS Infrastructure Lab | Cloud Computing & DevOps

📌 Project Overview

This project documents a hands-on AWS infrastructure lab focused on load balancing, EC2 instance provisioning, Auto Scaling, network security, and encryption key management.

The lab involved configuring an internet-facing Application Load Balancer (ALB), target groups, an EC2 launch template, an Auto Scaling Group (ASG), security groups, and an AWS Key Management Service (KMS) customer-managed key.

The objective was to gain practical experience with AWS compute, networking, scalability, and security services through the AWS Management Console.

Current status: The lab was completed, and the AWS resources have since been deleted to avoid ongoing infrastructure costs. The repository is maintained as project documentation; the deployed environment is no longer active.

🎯 Objectives

- Configure an Application Load Balancer for application traffic.
- Create a target group for registering application instances.
- Configure an EC2 launch template for instance provisioning.
- Create an Auto Scaling Group with configurable capacity.
- Configure security groups to control network access.
- Create a customer-managed KMS key and explore AWS key management.

🛠️ AWS Services Used

AWS Service| Purpose
Amazon EC2| Compute instances for application hosting
Application Load Balancer (ALB)| Routes incoming application traffic to registered targets
EC2 Auto Scaling| Manages the number of EC2 instances according to group settings and configured scaling policies
EC2 Launch Templates| Defines the configuration used to launch EC2 instances
Target Groups| Registers targets and performs health checks
Amazon VPC & Security Groups| Provides network isolation and traffic access control
AWS Key Management Service (KMS)| Creates and manages encryption keys

🏗️ Implementation

1. Application Load Balancer

- Created an internet-facing Application Load Balancer.
- Configured a target group for application targets.
- Configured security groups for network access.

2. EC2 Launch Template

- Created a launch template to define the configuration used when launching EC2 instances.
- Integrated the launch template into the Auto Scaling setup.

3. Auto Scaling Group

- Created an EC2 Auto Scaling Group named "mobile-ASG".
- Configured minimum, desired, and maximum capacity settings.
- Connected the Auto Scaling configuration to the load-balancing setup.

4. AWS Key Management Service (KMS)

- Created a customer-managed KMS key named "ec2-kms-key".
- Practiced the basic KMS key-management workflow.

Note: Creating a KMS key alone does not demonstrate that an EBS volume or other resource was encrypted using that key. This project does not claim verified resource encryption unless that configuration was actually implemented.

🧪 Validation & Evidence

The original AWS resources have been deleted, and the original deployment screenshots are no longer available. Therefore, the current AWS environment cannot be accessed to repeat the validation tests.

The following checks can be performed if the lab is recreated:

- Verify application accessibility through the ALB DNS endpoint.
- Check the health status of registered targets.
- Terminate an EC2 instance and verify whether the Auto Scaling Group replaces it.
- Test a configured scaling policy and observe changes in instance capacity.
- Verify resource encryption if a KMS encryption use case is configured.

These are suggested validation steps, not claims that every test was successfully completed during the original lab.

📚 Key Learning Outcomes

- Understanding the relationship between Application Load Balancers, target groups, launch templates, and Auto Scaling Groups.
- Learning how Auto Scaling capacity settings control EC2 instance provisioning.
- Understanding the role of security groups in network access control.
- Gaining introductory experience with AWS KMS and customer-managed keys.
- Practicing AWS resource configuration and management through the AWS Management Console.
- Understanding the importance of AWS cost management and resource cleanup.

🏗️ Architecture

The intended architecture consists of an internet-facing Application Load Balancer routing traffic to a target group of EC2 instances provisioned through a launch template and managed by an Auto Scaling Group.

KMS is documented as a separate key-management component. Its relationship to data encryption depends on the actual encryption configuration.

Note: The architecture can be represented using a diagram for explanatory purposes. Any such diagram should be identified as illustrative rather than as a screenshot or proof of a currently running deployment.

💰 Cost Management

AWS resources used in this lab may incur charges, including Application Load Balancers, EC2 instances, public IPv4 addresses, and KMS keys.

Cost-management practices include:

- Reviewing AWS pricing before deploying resources.
- Deleting unused infrastructure after completing the lab.
- Checking for remaining load balancers, EC2 instances, volumes, snapshots, and other billable resources.
- Reviewing KMS key deletion requirements before scheduling key deletion.
- Checking AWS Billing and Cost Management for any remaining charges.

👨‍💻 Author

Akash K

- GitHub: "Akash-k1" (https://github.com/Akash-k1)

Focus Areas: AWS Cloud, Cloud Support, DevOps, Infrastructure Management
