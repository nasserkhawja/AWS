# AWS
VPC and Subnet: A new VPC with a CIDR block of 10.0.0.0/16 and a subnet 10.0.1.0/24 is created.
Internet Gateway and Route Table: An internet gateway is created and attached to the VPC. A route table is created to route traffic to the internet.
Security Group: A security group (ssh_sg) is created allowing inbound SSH traffic (port 22) only from within the VPC (10.0.0.0/16). Outbound traffic is allowed to any destination.
EC2 Instances: 20 EC2 instances are created with the specified AMI and instance type. Each instance has a root EBS volume of 1TB (gp2 type).
Outputs: The public IP addresses of the created instances are outputted for reference.
Save the script to a .tf file, for example, main.tf.
Run terraform init to initialize the Terraform environment.
Run terraform apply to create the resources. You'll be prompted to confirm the operation.
