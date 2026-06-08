# Step 1

VPCs are isolated sections of AWS cloud that help to keep AWS Resources private & secure
When I set up my AWS Account, a default VPC is created to enable deployment of AWS Resources like EC2 Instances/RDS databases immediately
To set up a VPC, I defined an IPV4 CIDR which means a range of IP Addresses that my VPC can allocate to the resources deployed into my VPC.

<img width="997" height="725" alt="createvpc" src="https://github.com/user-attachments/assets/3655bd7b-3123-4b85-a6ad-49a444ecbb2b" />

# Step 2

Subnets are subdivisions within the VPC where we will launch resources
In the VPC dashboard under VPC select Subnets
Subnets are used to group resources with similar access rules & restrictions.
Some subnets might be public areas that all resources can access (Public Subnets)
Some are private areas with limited access (Private Subnet)

VPCs can have as many public & private subnets as needed.
Subnets in the same VPC cannot have overlapping IP Address CIDR Blocks
Each subnet must have a unique range of IP Address.

## AZs
Zoom out of the VPC. Each AWS Region is powered by a cluster of data centres dotted around the region
These clusters are Availability Zones
When i created the subnet within the VPC I assigned it to an Availability Zone instead of an entire region.
By spreading our resources across multiple AZs within the same region we are essentially creating a backup.
If one AZ faces issues, others can step up to keep the application running
