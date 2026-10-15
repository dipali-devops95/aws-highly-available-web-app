# Highly Available Web Application on AWS

## Project Overview

This project demonstrates how to build a highly available and secure web application infrastructure using Amazon Web Services (AWS).

The infrastructure includes a custom VPC, public and private subnets, an Internet Gateway, a Bastion Host, private EC2 web servers, an Application Load Balancer, and an Auto Scaling Group.

## Objectives

- Create a custom AWS VPC.
- Configure public and private subnets across two Availability Zones.
- Configure route tables and an Internet Gateway.
- Configure Security Groups for controlled access.
- Set up a Bastion Host for secure SSH administration.
- Deploy web servers in private subnets.
- Configure an Application Load Balancer.
- Configure an Auto Scaling Group.
- Test application availability and document the results.

## AWS Services

- Amazon VPC
- Amazon EC2
- Internet Gateway
- Route Tables
- Security Groups
- Application Load Balancer
- EC2 Launch Template
- Auto Scaling Group

## Architecture

Internet → Application Load Balancer → Private Web Servers

A Bastion Host provides administrative access to private instances.

## Project Documentation

Detailed implementation steps, verification results, and screenshots will be added to the `docs/` and `screenshots/` folders as the project progresses.

## Security

- Restrict SSH access to trusted IP addresses.
- Do not expose private web servers directly to the Internet.
- Allow web traffic through the Application Load Balancer.
- Never upload private keys, passwords, or AWS credentials to GitHub.

## Cost Management

AWS resources may incur charges depending on the service, region, and usage. Resources will be reviewed and cleaned up after testing.

## Project Status

In Progress
