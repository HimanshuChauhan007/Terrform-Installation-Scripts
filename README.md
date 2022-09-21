# demo_terraform
This repo contains a demo terraform code which can be used to test and understand how terraform operates.


Install Terraform - https://learn.hashicorp.com/tutorials/terraform/install-cli
**
Note – For windows follow the tutorial and then directly jump to step - https://www.youtube.com/watch?v=Cn6xYf0QJME**

•	If you’re using MacBook, create a file using $vi terraform.sh
•	Paste the script code in the file and save by pressing esc [Button] + wq! + Enter [Button]

    #!/bin/bash
    # dowload
    cd /tmp
    LATEST_TAG=$(curl -sL https://api.github.com/repos/hashicorp/terraform/releases/latest | grep tag_name)
    VERSION=$(echo $LATEST_TAG | grep -Eo "(\d+\.)+\d+")
    curl -OL https://releases.hashicorp.com/terraform/${VERSION}/terraform_${VERSION}_darwin_amd64.zip

    # install
    unzip terraform_${VERSION}_darwin_amd64.zip
    mv terraform /usr/local/bin/
**
Note – For Linux only change the code in the script rest of steps will remain the same.** 

    #!/bin/bash
    # dowload
    cd /tmp
    LATEST_TAG=$(curl -sL https://api.github.com/repos/hashicorp/terraform/releases/latest | grep tag_name)
    VERSION=$(echo $LATEST_TAG | grep -Eo "(\d+\.)+\d+")
    curl -OL https://releases.hashicorp.com/terraform/${VERSION}/terraform_${VERSION}_linux_amd64.zip

    # install
    unzip terraform_${VERSION}_linux_amd64.zip
    mv terraform /usr/local/bin/

•	Change the file permission using $chmod +x terraform.sh
•	Run the script $./terraform.sh
•	Verify terraform from any directory using $terraform –version
**
Note - Step 2 and Step 3 are not mandatory**

2.	Install AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
3.	Configure AWS CLI - https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html
Working with Code

1.	On MAC, open terminal and create a file using the command $vi main.tf and paste code mentioned in the Github repo.
2.	Save by pressing esc [Button] + wq! + Enter [Button]
3.	Create another file $vi terraform.tfvars and paste code from mentioned Github repo.
4.	Save the code by pressing ESC key and then typing $ wq!
5.	Jump to the directory location where you saved the files i.e., main.tf and terraform.tfvars
6.	Run $terraform init [To initiate terraform libraries]
7.	Run $terraform validate [To validate your code]
8.	Run $terraform plan [It will showcase what will be created]
9.	Run $terraform apply [It will create the infrastructure]
10.	Run $terraform destroy [It will destroy the created infrastructure]
