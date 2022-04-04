## Project 2 - HaiLT23 - Deploy a high-availability web app using CloudFormation
### How to deploy this project?
# Ensure that the AWS CLI is configured before runniing the command below and change the aws profile UdacityLab to your profile
## Windows
# create network
./deploy-server.bat create-vpc-project2 create-vpc.yml create-vpc-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create security group
./deploy-server.bat create-security-group create-security-group.yml create-security-group-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create iam role
./deploy-server.bat create-iam create-iam.yml create-iam-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create load balancer
./deploy-server.bat create-loadbalancer create-loadbalancer.yml create-loadbalancer-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create launch configuration
# Change the AMI ID, key-pair, bucket name, key of source code web app that stored at S3 in the create-launch-configuration.yml
./deploy-server.bat create-launch-configuration create-launch-configuration.yml create-launch-configuration-params.json ap-southeast-1 UdacityLab


## Linux/MacOS
# Ensure that the AWS CLI is configured before runniing the command below and change the aws profile UdacityLab to your profile
# create network
./deploy-server.sh create-vpc-project2 create-vpc.yml create-vpc-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create security group
./deploy-server.sh create-security-group create-security-group.yml create-security-group-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create iam role
./deploy-server.sh create-iam create-iam.yml create-iam-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create load balancer
./deploy-server.sh create-loadbalancer create-loadbalancer.yml create-loadbalancer-params.json ap-southeast-1 UdacityLab

# Waitting for the deployment of previous step to be completed
# create launch configuration
# Change the AMI ID, key-pair, bucket name, key of source code web app that stored at S3 in the create-launch-configuration.yml
./deploy-server.sh create-launch-configuration create-launch-configuration.yml create-launch-configuration-params.json ap-southeast-1 UdacityLab

### Visit my web site 
http://creat-elbwe-hom7pe2beoys-1661306197.ap-southeast-1.elb.amazonaws.com