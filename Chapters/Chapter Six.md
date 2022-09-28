# Chapter Six: Virtual Private Cloud

## Conceptual Overview of VPCs
---

### What Is a VPC? (Simplified)

A VPC (Virtual Private Cloud)  is a private subsection of AWS that you control, into which you can place AWS resources (such as EC2 instances and databases). You have **full** control over who has access to the AWS resources that you place inside your VPC.

### AWS Definition of a VPC:

Amazon Virtual Private Cloud lets you provision a **logically isolated** section of the Amazon Web Services (AWS) cloud where you can launch AWS resources in a **virtual network** that you define. **You have complete control over your virtual networking environment**, including selection of your own IP address range, creation of **subnets**, and configuration of **route tables** and **network gateways**.

### What Is a Subnet (Simplified):

A subnet (shorthand for "subnetwork") is a subsection of a network. Generally, a subnet includes all of the computers in a specific location.

### AWS Definition of a Subnet:

When you create a VPC, it spans all of the Availability Zones in the region. After creating a VPC, **you can add one or more subnets in each Availability Zone**. Each subnet **must reside entirely** within one Availability Zone and **cannot span zones**.

<br>

## Internet Gateways and Route Tables
---

### What Is an Internet Gateway? (Simplified)

A combination of hardware and software that provides your private network with a **route** to the world outside (meaning the internet) of the VPC.

### AWS Definition of an Internet Gateway

An internet gateway is a horizontally scaled, **redundant and highly available** VPC component that **allows communication between instances in your VPC and the internet**. It therefore imposes no availability risks or bandwidth constraints on your network traffic.

### What Is a Route Table

A route table contains a **set of rules**, called **routes**, that are used to **determine where network traffic is directed**.


### Networking Security

- **Network Access Control List (NACL)**
	- A firewall/security layer on the subnet level
- **Security Group (SG)**
	- A firewall/security layer on the instance/server level
- **What Is a Firewall?**
	- A firewall is a type of software that either allows or blocks certain kinds of internet traffic to pass through it.

<br>

## VPCs: Just the FAQs (Summary)
---

- A network can be compared to a neighborhood. The roads represent the network, and the houses represent the computers on the network.
- The cars represent the data moving through the network. When a car (data) leaves the neighborhood (network), it is destined for another network.
- A single street with houses represents a subnet with computers.
- A VPC is a private part of the AWS cloud that customers create to hold AWS resources they wish to use.
- A default VPC is created when a new AWS account is created.
- Multiple VPCs may be created.
- VPCs cross Availability Zones
- Subnets are created within a VPC
- Subnets may be public or private
- Private subnets do not have access to the internet, but public subnets do have access to the internet (assuming a route table with a route to the internet gateway exists) The terms "public" subnet and "private" subnet are labels
- A route/no route to the  IGW is what makes a subnet public or private
- An internet gateway provides internet connectivity. IGWs may be attached to and detached from a VPC.
- Route tables are used to direct traffic to various destinations. Route tables may or may not have a route to an IGW.
- Security (firewall security) is provided by the NACL and the security group, NACLs have rules to allow traffic into and out of subnets. A NACL can be assigned to one or more subnets.

<br>

## Virtual Private Cloud (Quiz / Correct answers only!)

- **A subnet is a _____.**
	- Subsection of a network
- **In this scenario, we have a NACL with the following rules, Which is true based on the rules within this NACL?** 

            Rules	Traffic 
            Rule#1	Allow SSH 
            Rule#2	Allow HTTP 
            Rule#3	Deny All 
            Rule#4	Allow All 
            
	- All traffic except SSH and HTTP will be denied
- **How many subnets are created by default in each region when an AWS account is created?**
	- 1 subnet per Availability Zone
- **Which of the following is descriptive of an Internet Gateway?**
	- A route to and from the internet
- **A security group is a _ on the _ level.**
	- Firewall, instance
- **What is a NACL?**
	- A firewall on the subnet level
- **Which of the following will create subsections of a VPC?**
	- Subnet
- **Which of these statements is true of subnets?**
	- We can add one or more subnets in each AZ.
	- The default VPC already has subnets created for each AZ by default.
	- Subnets cannot span AZs.
- **Which of the following is true about subnets?**
	- Subnets cannot span AZs
- **Which of the following are true statements about public subnets and private subnets?**
	- A private subnet does not have a route table pointed to an Internet Gateway
	- A public subnet has a route table pointing to an Internet Gateway
- **What does a route table do?**
	- Directs traffic within a network
- **How many VPCs can an EC2 instance be attached to at a time?**
	- 1