# Create-a-VPC-Endpoint-and-S3-Bucket-in-AWS
This is simple demonstration on accessing S3 bucket using EC2 instance in private subnet. This project highlights the key difference between VPC endpoint and NAT gateway.

# Which is preffered to connect private subnet to open internet - VPC endpoint or NAT gateway?
--> VPC endpoint provides better performance and more secure connection as it does not use public subnet to connect to outside internet like NAT Gateway does.
--> NAT gateway is highly scalable and available as it resides in public subnet to connect private subnet to outside internet

# Demonstration
1.	Create VPC
2.	Create 2 subnet- public & private
3.	Create 2 EC2 instances – public & private 
4.	Create 2 Route table – public & private
5.	Create Internet Gateway and add it to public route table
6.	Create S3 bucket
7.	Create VPC endpoint by selecting S3 service and adding private Route table.
8.	Verify additional record of route referring S3 is added under private Route table.
9.	Access S3 using private EC2 instance via SSh terminal


