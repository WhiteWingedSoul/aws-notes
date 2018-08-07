# Introduction to Amazon VPC
## Introduction
- A private virtual network in the AWS Cloud
    - Uses same concepts as on premise networking
- Allow complete control of network configuration
    - Ability to isolate and expose resources inside VPS
- Offers several layers of security controls
    - Ability to allow and deny specific internet and internal traffic
- Other AWS services deploy into VPC
    - Service inherent security built into network

## Features
- Builds upon high availability of AWS Regions and Availability Zones
    - VPC lives within a Region
    - Multiple VPCs per account

## Subnets
- Used to divide Amazon VPC
- Allows Amazon VPC to span multiple Azs

## Route tables
- Control traffic going out of the subnets

## Internet Gateway (IGW)
- Allows access to the internet from Amazon VPC

## NAT Gateway
- Allows private subnet resources to access Internet

## Network Access Control Lists (NACL)
- Control access to subnets; stateless