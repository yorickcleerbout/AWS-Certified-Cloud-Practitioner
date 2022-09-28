# Chapter Nine: ELB and Auto Scaling

## Elastic Load Balancing (ELB)
---

### What Is Elastic Load Balancing (ELB)? (Simplified)

An ELB evenly distributes traffic between EC2 instances that are associated with it.


### AWS Definition of ELB

A load balancer **distributes incoming application traffic across multiple EC2 instances in multiple Availability Zones.** This **increases the fault tolerance** of your applications. Elastic Load Balancing **detects unhealthy instances and routes traffic only to healthy instances.**

<br>

## Auto Scaling
---

### What Is Auto Scaling? (Simplified)

Auto Scaling automates the process of adding (**scaling up**) or removing (**scaling down**) EC2 instances **based on traffic demand** for your application.

### AWS Definition of Auto Scaling

Auto Scaling helps you ensure that you have the correct number of Amazon EC2 instances available to **handle the load for your application**. You create collections of EC2 instances, called **Auto Scaling groups**. You can specify the minimum number of instances in each Auto Scaling group, and Auto Scaling ensures that your group never goes below this size. You can specify the maximum number of instances in each Auto Scaling group, and Auto Scaling ensures that your group never goes above this size. If you specify the desired capacity, either when you create the group or at any time thereafter, Auto Scaling ensures that your group has this many instances. If you specify scaling policies, then auto scaling can launch or terminate instances as demand on your application increases or decreases.

<br>

## ELB and Auto Scaling: Just the FAQs (Summary)
---

- Elastic Load Balancing evenly distributes traffic between EC2 instances that are associated with it.
- ELB can distribute traffic across multiple instances across multiple Availability Zones, which increases application fault tolerance.
- ELB can detect unhealthy instances and redirect traffic to healthy instances.
- Auto Scaling automates the process of scaling up and scaling down EC2 instances based on traffic demands.
- Auto Scaling adds scalability and elasticity to ELB.

<br>

## ELB and Auto Scaling: Quiz (Correct answers only!)
---

- **Which of the following Cloud concepts correlate with an Auto Scaling Group?**
	- Scalability
	- Elasticity
- **We have 3 EC2 instances and notice that traffic is routing to only one EC2 instance. Which of the following will allow us to distribute traffic amongst the EC2 instances?**
	- ELB
- **An Auto Scaling Group is a _____.**
	- Logical grouping of EC2 instances for the purpose of scaling
- **An ELB is a __.**
	- Load Balancer