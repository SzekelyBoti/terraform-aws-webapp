## EC2 Web Application Deployment with Terraform

# Overview

    This project streamlines the deployment of a web application on an AWS EC2 instance using Terraform.
    The objective is to facilitate a robust and efficient setup process for hosting a web application.
    The project leverages Terraform for infrastructure as code, utilizes AWS EC2 for scalable hosting solutions, and is based on Ubuntu Server as the operating system.

# Prerequisites

    An active AWS account to provision resources.
    AWS CLI configured with appropriate permissions to manage EC2 instances.
    Terraform installed on your local machine for infrastructure provisioning.

# Usage

- To deploy the project, please follow these steps:
  Clone the Repository:

  git clone <https://github.com/SzekelyBoti/terraform-aws-webapp.git>
  
  cd <terraform-aws-webapp>

  Update Configuration: Modify the main.tf file to reflect your desired configurations, including the appropriate AMI ID and instance type.

  Initialize Terraform: Execute the following command to initialize your Terraform working directory:

  terraform init

  Review the Deployment Plan: Create an execution plan to review the proposed changes:

  terraform plan

  Apply the Configuration: Proceed with the deployment of the EC2 instance and associated resources:

  terraform apply

  Confirm the action by entering yes when prompted.

  Access Your Web Application: After deployment is complete, you can access your web application by navigating to the public IP address of your EC2 instance in your web browser.

# Example Outputs

- Upon successful deployment, the output will resemble the following:
  Apply complete! Resources: 1 added, 0 changed, 0 destroyed.
- Outputs:

  instance_ip = "your-instance-public-ip"

- Accessing http://<your-instance-public-ip>/ in a web browser will present the web application hosted on your EC2 instance.
