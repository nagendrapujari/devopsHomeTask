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

1.**Configure AWS Credentials.** <br>
Set up your AWS credentials using the AWS CLI: <br>
$aws configure <br>
enter acces id and key when prompts:

2. **Customize the Configuration**

Open the main.tf file and update the following placeholders to match your environment:

'cidr_block' in 'aws_vpc' and 'aws_subnet' with your desired IP ranges.

'ami' in 'aws_instance' with your preferred Amazon Machine Image ID.

'filename' in 'aws_lambda_function' with the path to your Lambda function deployment package.

'TARGET_GROUP_ARN' in 'aws_lambda_function' with your Network Load Balancer target group ARN.

3. **Initialize Terraform**

Initialize Terraform to download provider plugins and set up the working directory:
$terraform init

4. **Review the Execution Plan**

Generate and review an execution plan to ensure Terraform will make the expected changes:

$terraform plan

5. **Apply the Configuration**

Apply the configuration to create the resources:

$terraform apply

Confirm the action by typing 'yes' when prompted.

To view the current state of your infrastructure:

$ terraform show list





