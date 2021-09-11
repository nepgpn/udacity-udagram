# udacity-udagram
This script creates VPC, Public and Privates subnets, securitygroups , and ec2 instances for web servers and a bastion host for access the webservers.

Following files in the dir.
1. udagram.yml
2. parameters.json
3. design diagram
4. screen shot of the page.
5. loadbalancer output 




Run the command to generate the resource 

aws cloudformation create-stack  --stack-name udagramstack --region us-east-2 --template-body file://udagram.yml --parameters file://parameter.json --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM"


Run the coomand to destroy the resource.
aws cloudformation delete-stack --stack-name udagramstack 