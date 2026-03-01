# AWS-VPC-Secure-Network-Architecture
Secure AWS VPC design with public and private subnets
--Project Overview
- This Project demonstrates the design and implementation of a secure AWS Virtual Private Cloud (VPC) architecture.  The infrastructure includes public and private subnets, controlled internet access, and multiple security layers following AWS best practices.

- The goal of this project is to build a secure, scalable, and production-ready network enviornment

--Tools & Services Used
- AWS VPC
- Amazon EC2
- Internet Gateway(IGW)
- Route Table
- Security Groups

--Architecture Design
- Custom VPC CIDR 10.0.0.0/16
- Public Subent 10.0.1.0/24
- Private Subnet 10.0.2.0/24
- Public EC2 Instance (Web Server)
- Private EC2 Instance (Application Server)
- Internet Gateway for Public access
- NAT Gateway for Private Subnet outbound access

--Security Implementation
- SSH access restricted to specific IP address
- Ppublic and private subnet separtaion
- Security Groups for instance-level firewall control
- Private Instances do not have public IP address

-- Routing Configuration
- Public Route Table  0.0.0.0--> Internet Gateway
- Private Route Table 0.0.0.0--> NAT Gateway

  --Testing & Validation
  - SSH Connectivity to public instance
  - SSH from public instance to private instance
  - Internet access test from private subnet via NAT
  - HTTP webserver validation
  - Traffic monitoring using VPC Flow Logs.

- 
