# demo_terraform
This repo contains a demo terraform code which can be used to test and understand how terraform operates.


Install Terraform - https://learn.hashicorp.com/tutorials/terraform/install-cli

Note – For windows follow the tutorial and then directly jump to working with the code section - https://www.youtube.com/watch?v=Cn6xYf0QJME

    •	If you’re using MacBook, download and run the script - macbook.sh

Note – For Linux, download and run the script - linux.sh

    •	Change the file permission using $chmod +x macbook.sh
    •	Run the script $./macbook.sh
    •	Verify terraform from any directory using $terraform –version

**Note - Step 2 and Step 3 are not mandatory**

2.	Install AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
3.	Configure AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html

**Working with Code**

1.	Download the files, main.tf and terraform.tfvars and place them in a folder/directory or choice
2.	Jump to the directory or folder location on the terminal where you saved the files i.e., main.tf and terraform.tfvars
3.	Run $terraform init [To initiate terraform libraries]
4.	Run $terraform validate [To validate your code]
5.	Run $terraform plan [It will showcase what will be created]
6.	Run $terraform apply [It will create the infrastructure]
7.	Run $terraform destroy [It will destroy the created infrastructure]
