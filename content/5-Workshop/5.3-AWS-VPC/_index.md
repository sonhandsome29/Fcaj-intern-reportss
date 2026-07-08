---
title : "Set Up the Virtual Network (AWS VPC)"
date : 2026-07-04
weight : 3
chapter : false
pre : " <b> 5.3. </b> "
---

In this section, we manually create an **Amazon VPC** to provide a secure networking foundation for the project. Instead of using the default VPC, we build a simple layered network architecture that includes:

* one **public subnet** for the backend EC2 instance
* two **private subnets** for the RDS database
* an **Internet Gateway**
* separate **Route Tables** for public and private traffic

This design helps keep the database isolated from the public internet while still allowing the backend server to be deployed and managed easily.

#### Contents

1. [Create the VPC and Subnets](5.3.1-create-vpc-subnets/)
2. [Configure the Internet Gateway and Route Tables](5.3.2-igw-route-tables/)
