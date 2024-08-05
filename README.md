# devopsHomeTask
DevopsHomeTask
This repository contains a Terraform configuration to deploy a basic infrastructure setup on AWS. The setup includes a Virtual Private Cloud (VPC), a subnet, an Internet Gateway, a Security Group, an EC2 instance, a Network Load Balancer (NLB), an AWS Lambda function, and associated IAM roles and policies.

Overview
The script provisions the following AWS resources:

VPC - A Virtual Private Cloud for network isolation.
Subnet - A public subnet within the VPC.
Internet Gateway - Allows access to the internet from the VPC.
Route Table - Routes internet traffic through the Internet Gateway.
Security Group - Configures firewall rules for inbound and outbound traffic.
EC2 Instance - A virtual server running Amazon Linux 2 with Nginx.
Network Load Balancer - Distributes traffic across multiple targets.
Lambda Function - A serverless function triggered every 5 minutes.
IAM Roles and Policies - Required for Lambda execution and permissions.
Prerequisites
Before running the Terraform script, ensure you have:

Terraform installed (version X.X.X or later).
AWS CLI installed and configured with appropriate credentials.
An AWS account with permissions to create and manage the specified resources.

