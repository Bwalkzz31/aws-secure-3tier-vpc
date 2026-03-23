AWS Secure 3-Tier Architecture and SSH Hardening.

## Overview

The project illustrates how to design and deploy a secure 3-tier cloud infrastructure in AWS. Best practices were used to configure the environment with the network segmentation, access control, and more secure administrative access.

The architecture isolates resources into the public and private layers and implements least-privilege access using security groups and SSH.

## Objective

In order to create a secure AWS environment that:

* Layer network (web, application, database) segmentation.
* Denies unauthorized access with security groups.
* Gains access to the administration using SSH keys.
* Shows actual cloud security.

## Architecture Design

The infrastructure has three levels:

* **Public Subnet (Web Layer)– Houses resources that are internet-facing.
* **Privatized Subnet (Application Layer) - Internal application logic.
* **Private Subnet (Database Layer) The database layer is a secure storage of data without direct access by the population.

## Key Features

* Created a custom VPC with subnets.
* Established security groups with least privilege access.
* Enacted key-based authentication in gaining remote access with SSH keys.
* SSH access to one trusted IP address.
* Implemented and tested a web server on the public subnet.
* Denied access to private resources.

## Security Implementation

SSH access is limited to authorized IP.
* Private key is kept in a safe location and is not shared.
* Security groups in the form of virtual firewalls.
* Network segmentation minimizes attack surface.
* No open application or database layers.

## SSH Configuration

An EC2 access was secured with a key pair. Only a single IP address was allowed to enter into the environment via SSH, which guaranteed controlled administrative access to the environment.

📄 See detailed configuration:

* ssh-access-configuration.pdf

## Screenshots

### Web Server Deployment

![Web Server](screenshots/web-server.png)

The 3-tier architecture Diagram shown below presents a secure architecture implementation.

![Architecture](architecture-diagram.png)

## Technologies Used

* AWS (VPC, EC2, Security Groups)
Key-based Authentication (SSH) involves the use of keys to access a system or network.<|human|>* SSH (Key-Based Authentication)
! Key-based Authentication (SSH) is a system or network that uses keys to access the system.
* Concepts of Networking (CIDR, Subnets)
Cloud Security Best Practices.

## Outcome

This project reveals the capability to design and secure cloud infrastructure with the help of AWS. It emphasizes the abilities of network segmentation, access control, and secure system administration.

## Relevance

The project applies to the work in:

* IT Support
* Systems Administration
* Cloud Engineering
* Cybersecurity

---
 Created by Britany Walker
IT Support Systems Administration Cybersecurity.
