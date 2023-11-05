# Terraform Infrastructure as Code (IaC)

This repository contains Terraform scripts for managing cloud infrastructure. It uses Terraform to provision and manage resources declaratively with versioned configuration files.

## Pre-requisites

Before you can use these Terraform scripts, ensure you have the following installed and configured:

- **Terraform:** You should have the latest version of Terraform installed on your system. Visit [Terraform's website](https://www.terraform.io/downloads.html) for download and installation instructions.
- **Cloud Provider CLI:** Since these scripts are designed for use with the cloud provider Microsoft Azure, make sure you have the respective CLI installed and authenticated on your local machine.
- **Git:** As we're using Git for version control, make sure you have it installed. Refer to [Git's website](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) for installation instructions.
- **SSH Key:** Ensure you have an SSH key pair generated for secure communication with the Git repository.


## How to Use

To use the Terraform scripts, you can follow these steps:

1. **Clone the Repository:**
git clone https://github.com/jenserling/iac-oppgave2.git
   
2. **Initialize Terraform:**
Run "terraform init" command to initialize Terraform, it will download necessary providers and modules.

3. **Create a Terraform Plan:** (Optional)
To see what Terraform will do before actually making any changes, run: "terraform plan"

4. **Apply the Terraform Configuration:**
To apply the configuration and create the resources, run: "terraform apply" And you'll be prompted to confirm the action before Terraform proceeds to make any changes to your infrastructure.

5. **Inspect State:**
After applying, you can inspect the current state of your resources using: "terraform show"

6. **Destroy Infrastructure:**
When you no longer need the resources, you can destroy them with: "terraform destroy" again, you'll be prompted to confirm the action before Terraform deletes anything.

## Continuous Integration / Continuous Deployment (CI/CD)
This repository is also equipped with GitHub Actions workflows for CI/CD, automatically running Terraform tests, and applying configurations when changes are merged into specific branches. To utilize these workflows, ensure your GitHub repository secrets are configured with the necessary credentials and SSH keys.








