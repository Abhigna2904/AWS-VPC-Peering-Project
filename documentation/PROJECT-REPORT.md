# AWS VPC Peering – Project Report

## 1. Introduction
This project focuses on private communication between two AWS Virtual Private Clouds using VPC Peering.

## 2. Problem Statement
Two separate VPCs need to communicate privately without routing traffic through the public internet.

## 3. Proposed Architecture
- VPC A: 10.10.0.0/16
- VPC B: 10.20.0.0/16
- Public and private subnets
- Three EC2 instances
- One VPC Peering connection

## 4. AWS Services Used
- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- Internet Gateway

## 5. Implementation
The implementation will include VPC creation, subnet configuration, EC2 deployment, security group configuration, VPC Peering, and route table updates.

## 6. Testing
Connectivity will be tested between the private EC2 instances using their private IP addresses.

## 7. Current Status
GitHub repository and initial documentation have been created.

AWS resource creation and connectivity testing are pending access to an approved AWS lab environment.

## 8. Conclusion
This project demonstrates the concepts and planned implementation of private connectivity between two AWS VPCs.
