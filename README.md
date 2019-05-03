# WebServer-AWS-byAnsible
project ansible to launch a webserver httpd into AWS(ap-southeast-2)  


# Environment
The description below has been used to create as kick out to run the playbook ansible 

## Requirements
 ### System 
 Amazon Linux 2 AMI
 ### Ansible
 Ansible 2.7.10
 ### Python 
 python 2.7.14
 ### Boto
 boto 2.49.0, 
 boto3 1.9.140, 
 botocore 1.12.140
 ### SSH
 ssh-agent (ensure agent is runing) 

 + how to install:

 Ansible:
 https://aws.amazon.com/pt/blogs/mt /running-ansible-playbooks-using-ec2-systems-manager-run-command-and-state-manager/

 pip
 https://docs.aws.amazon.com/pt_br/cli/latest/userguide/install-linux.html

 boto3
 https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html



# Step one - Credentials
 Ensure you already have credentials set on: 

  ~/.aws/config  

  ~/.aws/credentials  

 How to set credentials up:

 $ aws configure 

# Step two - Repository
 Download of this repo and run this project

 $ git clone https://github.com/Renatovnctavares/WebServer-AWS-byAnsible.git   

# Step three - Running
 Run this project inside of the "WebServer-AWS-byAnsible" directory:

 $ ansible-playbook -i inventory project.yml


# Step four - Check out
 check out the acess URL into the file created.

 $ cat url_loadbalance_httpd.txt