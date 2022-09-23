# demo_terraform
This repo contains a demo terraform code which can be used to test and understand how terraform operates.


Install Terraform - https://learn.hashicorp.com/tutorials/terraform/install-cli

Note – For windows follow the tutorial and then directly jump to working with the code section - https://www.youtube.com/watch?v=Cn6xYf0QJME

    •	If you’re using MacBook, download and run the script - terraform_install_macos.sh

Note – For Linux, download and run the script - terraform_install_linux.sh

    •	Change the file permission using $chmod +x terraform_install_macos.sh
    •	Run the script $./terraform_nstall_macos.sh
    •	Verify terraform from any directory using $terraform –version

**Note - Step 2 and Step 3 are not mandatory**

2.	Install AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
3.	Configure AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html

**Working with Code**

1.	Create a role in AWS with programmatic access [terraform_admin], assign the necessary permissions for the services you wish to deploy and save the credentials file securely 
2.	Download the files, main.tf and terraform.tfvars from this repo and place them in a folder/directory of choice
3.	Jump to the directory or folder location on the terminal where you saved the files i.e., main.tf and terraform.tfvars
4.	Provide your AWS credentials by running below mentioned commands in terminal

      •   export AWS_ACCESS_KEY_ID=”access key”
      •	  export AWS_SECRET_ACCESS_KEY=”secret key”
      •	  export AWS_REGION=”us-east-1”
        
5.	Run $terraform init [To initiate terraform libraries]
6.	Run $terraform validate [To validate your code]
7.	Run $terraform plan [It will showcase what will be created]
8.	Run $terraform apply [It will create the infrastructure]
9.	Run $terraform destroy [It will destroy the created infrastructure]
