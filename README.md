# devopsHomeTask
DevopsHomeTask
This repository contains a Terraform configuration to deploy a basic infrastructure setup on AWS. The setup includes a Virtual Private Cloud (VPC), a subnet, an Internet Gateway, a Security Group, an EC2 instance, a Network Load Balancer (NLB), an AWS Lambda function, and associated IAM roles and policies.

**Overview**

The script provisions the following AWS resources:

1.**VPC** - A Virtual Private Cloud for network isolation.<br>
2. **Subnet** - A public subnet within the VPC.<br>
3. **Internet Gateway** - Allows access to the internet from the VPC.<br>
4. **Route Table** - Routes internet traffic through the Internet Gateway.<br>
5.**Security Group** - Configures firewall rules for inbound and outbound traffic.<br>
6.**EC2 Instance** - A virtual server running Amazon Linux 2 with Nginx.<br>
7.**Network Load Balancer** - Distributes traffic across multiple targets.<br>
8.**Lambda Function** - A serverless function triggered every 5 minutes.<br>
9.**IAM Roles and Policies** - Required for Lambda execution and permissions.<br>


**Prerequisites**

Before running the Terraform script, ensure you have:

Terraform installed (version X.X.X or later).<br>
AWS CLI installed and configured with appropriate credentials.<br>

**Setup Instructions:**

1.**Configure AWS Credentials.**
Set up your AWS credentials using the AWS CLI:
aws configure
enter acces id and key when prompts:





