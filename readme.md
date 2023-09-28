
# Basic AWS VPC Terraform Example

This repository contains a basic Terraform example that creates an Amazon Virtual Private Cloud (VPC) in AWS. This README provides instructions on how to use the example and what it does.

## Prerequisites

Before you begin, make sure you have the following prerequisites:

1. [Terraform](https://www.terraform.io/downloads.html) installed on your local machine.
2. AWS account credentials configured with the necessary permissions.

## Usage

Follow these steps to use this Terraform example:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/basic-aws-vpc-terraform.git
   ```

2. Change into the project directory:

   ```bash
   cd basic-aws-vpc-terraform
   ```

3. Create a `terraform.tfvars` file in the project directory to specify the required variables. You can use the following template as a starting point:

   ```hcl
   # terraform.tfvars

   vpc_cidr_block = "10.0.0.0/16"
   ```

   Replace `"10.0.0.0/16"` with your desired CIDR block for the VPC.

4. Initialize the Terraform project:

   ```bash
   terraform init
   ```

5. Review the Terraform execution plan to ensure you understand the changes that will be made:

   ```bash
   terraform plan
   ```

6. Apply the Terraform configuration to create the AWS VPC:

   ```bash
   terraform apply
   ```

   Terraform will prompt you to confirm the changes. Type `yes` and press Enter to proceed.

7. Wait for Terraform to provision the VPC and its resources. Once completed, you will see a message indicating success.

8. To destroy the created resources, run:

   ```bash
   terraform destroy
   ```

   This will remove the VPC and all associated resources.

## What It Does

This Terraform example creates an AWS VPC with the following characteristics:

- CIDR block: The CIDR block for the VPC is specified in the `terraform.tfvars` file.
- DNS Support and Hostnames: DNS support and DNS hostnames are enabled for the VPC.

## Author
Ayoub Umoru

