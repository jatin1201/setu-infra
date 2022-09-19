
Lets follow the below steps to execute the code 

Prerequisites 
- AWS Account 
- Terraform 
- Add aws profile name in the provider.tf
- AWS CLI must be configured 
- SSH Key (must be created prior execution of the code)
- Change variables.tf if needed (just in case you need to change some naming conventions this is totally optional)

Before executing the code lets understand bit of this code, i followed the terraform module approach (A group of Terraform configuration files contained in a single directory constitute a Terraform module. even a straightforward configuration with a single directory and one or more. A module is tf files. It is regarded as the root module when Terraform commands are executed directly from such a directory.) to launch our desired infrastruture over the aws 

This code is reusable and easy to setup.


Run the code 

- Clone this github repo
- cd into Terraform-setu

Once we inside the Setu directory as i mention we are using terraform module so we need to install all the modules of our infrastructure, to do so

- run terraform init
this will take couple minutes to insatalled all the modules into root 

- after the successful execution of init we need to test our code via dry run or more of validation of the code need to done 

- for that run terraform plan 
This will also take few mooment to load up and generate the output

once you validate the code successfully we need to enforce the changes to the aws account 
- run terraform apply 
this will take sometime to compelete the process and once it done you'll have your assets ready 

just log into the aws account >> switch your region >> check all the assets on the aws console








