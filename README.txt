# create network
./deploy-server.bat create-vpc-project2 create-vpc.yml create-vpc-params.json ap-southeast-1 UdacityLab

# create security group
./deploy-server.bat create-security-group create-security-group.yml create-security-group-params.json ap-southeast-1 UdacityLab

# create iam role
./deploy-server.bat create-iam create-iam.yml create-iam-params.json ap-southeast-1 UdacityLab

# create load balancer
./deploy-server.bat create-loadbalancer create-loadbalancer.yml create-loadbalancer-params.json ap-southeast-1 UdacityLab

# create launch configuration
./deploy-server.bat create-launch-configuration create-launch-configuration.yml create-launch-configuration-params.json ap-southeast-1 UdacityLab
