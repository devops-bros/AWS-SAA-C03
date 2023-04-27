# Create VPC
Name: MyVPC-PROD
IPv4 CIDR Block: 10.1.0.0/16

# Create Subnets

Name: Public-1A
Availability Zone: us-east-1a
IPv4 CIDR Block: 10.1.1.0/24

Name: Public-1B
Availability Zone: us-east-1b
IPv4 CIDR Block: 10.1.2.0/24

Name: Private-1A
Availability Zone: us-east-1a
IPv4 CIDR Block: 10.1.3.0/24

Name: Private-1B
Availability Zone: us-east-1b
IPv4 CIDR Block: 10.1.4.0/24

# Create private route table

Name: Private-RT
VPC: MyVPC-PROD
Subnet associations: Private-1A, Private-1B

# Create Internet Gateway

Name: MyIGW-PROD
VPC: MyVPC-PROD

# Account ID
821791694623


# VPC ID
vpc-09634272a333a4719


# Instance IP (Prod)
10.1.1.109

