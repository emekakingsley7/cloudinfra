# Basic Infrastructure Deployment on AWS using Terraform

## Overview

This project provisions and manages AWS infrastructure using Terraform. The infrastructure includes resources such as EC2 instances, VPC, and more. The goal is to provide a scalable, secure, and efficient cloud environment for deploying applications and services.

## Prerequisites

-Visual Studio Code insattled on local machine
- [Terraform] installed on VS code.
- AWS account with sufficient permissions to create and manage resources.
- AWS CLI configured with appropriate credentials.

## Infrastructure Components

The following AWS resources are provisioned by this Terraform configuration:

- **EC2 Instances**: Virtual servers to run applications.
- **VPC and Subnets**: Network infrastructure for resource isolation and security.
- **Security Groups**: Firewall rules to control inbound and outbound traffic.
- **NAT and Internet Gateways**: For internet access and control of traffick to in and out of the network.

## Getting Started

### Clone the Repository

```sh
git clone https://github.com/yourusername/your-repo.git
cd your-repo

## Getting Started

### Initialize Terraform
Initialize the Terraform working directory.


```terraform init
   ```
### Review and Apply the Configuration
Review the Terraform plan to see what resources will be created.

```terraform plan
   ```
If everything looks good, apply the configuration to create the resources.

```terraform apply
   ```
### Destroy the Infrastructure
When the resources are no longer needed and in order to avoid charges, the infrastructures were all destroyed.

```terraform destroy
   ```

### Terraform Files

Though I only used "main.tf" files but here are some files normally used in Terraform
- main.tf: The main Terraform configuration file that defines the resources to be created.
- variables.tf: File containing variable definitions used in the configuration.
- outputs.tf: File defining the outputs of the Terraform configuration.
- provider.tf: File specifying the provider (AWS in this case) and required versions.


### Troubleshooting
Encountering issues while coding is normal, here is some check that can help:

- Ensure AWS credentials are correctly configured.
- Verify that there are necessary permissions to the user to create and manage the resources.
- Review the Terraform documentation for specific resource requirements and configurations.
- Check for forums like Stackoverflow and or other community forum for help
