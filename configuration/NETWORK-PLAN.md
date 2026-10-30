# AWS VPC Peering – Network Configuration Plan

## 1. VPC Configuration

| Resource | CIDR Block |
|---|---|
| VPC A | 10.10.0.0/16 |
| VPC B | 10.20.0.0/16 |

## 2. Subnet Configuration

| Subnet | CIDR Block | VPC |
|---|---|---|
| Public Subnet A | 10.10.1.0/24 | VPC A |
| Private Subnet A | 10.10.2.0/24 | VPC A |
| Private Subnet B | 10.20.1.0/24 | VPC B |

## 3. EC2 Instance Plan

| Instance | Private IP |
|---|---|
| Bastion Host | 10.10.1.10 |
| App-A | 10.10.2.10 |
| App-B | 10.20.1.10 |

## 4. VPC Peering Routes

| Route Table | Destination | Target |
|---|---|---|
| VPC A Private | 10.20.0.0/16 | VPC Peering |
| VPC B Private | 10.10.0.0/16 | VPC Peering |
| VPC A Public | 10.20.0.0/16 | VPC Peering |

## 5. Network Security

- Bastion SSH access should be restricted to the user's public IP.
- App-A and App-B SSH access should be restricted to the bastion host.
- ICMP traffic should be allowed between App-A and App-B for connectivity testing.

**Note:** This is the planned configuration from the project workbook. Actual AWS configuration is pending practical implementation.
