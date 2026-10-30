# AWS VPC Peering Project

## Project Overview

This project focuses on establishing private network communication between two Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering.

The objective is to understand VPC creation, subnet configuration, EC2 deployment, route tables, security groups, and private communication between two VPCs.

## Objectives

- Create two separate VPCs.
- Configure public and private subnets.
- Deploy EC2 instances.
- Configure security groups.
- Establish a VPC Peering connection.
- Update route tables to enable private communication.
- Test connectivity between instances.

## Architecture and IP Address Plan

| Resource | CIDR / Private IP |
|---|---|
| VPC A | 10.10.0.0/16 |
| Public Subnet A | 10.10.1.0/24 |
| Private Subnet A | 10.10.2.0/24 |
| VPC B | 10.20.0.0/16 |
| Private Subnet B | 10.20.1.0/24 |
| Bastion Host | 10.10.1.10 |
| App-A | 10.10.2.10 |
| App-B | 10.20.1.10 |

## AWS Services and Technologies

- Amazon Virtual Private Cloud (VPC)
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- Amazon Linux
- SSH

## Implementation Steps

1. Create VPC A and VPC B.
2. Create the required subnets.
3. Configure the Internet Gateway for VPC A.
4. Create and configure route tables.
5. Configure security groups.
6. Deploy the EC2 instances.
7. Establish the VPC Peering connection.
8. Update routes in both VPCs.
9. Test private connectivity.

## Testing and Validation

The planned validation includes:

- Checking the VPC Peering connection status.
- Verifying route table entries.
- Testing private IP connectivity between App-A and App-B.
- Checking security group restrictions.

## Current Project Status

**Documentation and GitHub repository:** Created.

**AWS implementation and connectivity testing:** Pending free lab access and practical execution.

Actual AWS resource IDs, screenshots, and test results will be added after implementation.

## Learning Outcomes

This project is intended to provide practical knowledge of AWS networking, private communication, cloud infrastructure, and network security.

## References

- EWB AWS VPC Peering Student Project Workbook.
- EWB AWS Cloud Computing Training Notes.
- AWS Documentation: https://docs.aws.amazon.com/
