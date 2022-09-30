# Chapter Seventeen: AWS Pricing, Billing, and Support Services

## AWS Organizations
---

### What Are AWS Organizations? (Simplified)

Organizations allow you (or your company) to manage billing and access to multiple AWS accounts (in one user interface).

### AWS Definition of AWS Organizations

AWS Organizations offer **policy-based management for multiple AWS accounts**. With Organizations, you can create groups of accounts and then apply policies to those groups. **Organizations enables you to centrally manage policies across multiple accounts**, without requiring custom scripts and manual processes. Using AWS Organizations, you can create **Service Control Policies (SCPs) that centrally control AWS service use across multiple AWS accounts**. You can also use Organizations to help **automate the creation of new accounts through APIs**. Organizations helps **simplify the billing for multiple accounts** by enabling you to set up a single payment  method for all the accounts in your organization through consolidated billing. AWS Organizations is available to all AWS customers at no additional charge.

- **Main Features/Benefits**:
	- Centrally manage access policies across multiple AWS accounts
	- Control access to AWS services
	- Automate AWS account creation and management
	- **Consolidated billing** across multiple AWS accounts

### What Is Consolidated Billing (Simplified)

Consolidated billing allows you to view, manage, and pay bills for multiple AWS accounts in one user interface.

### AWS Definition of Consolidated Billing

AWS Organizations **enables you to set up a single payment method for all the AWS accounts in your organization** through consolidated billing. With consolidated billing, you can see a combined view of charges incurred by all your accounts, **as well as take advantage of pricing benefits from aggregated usage**, such as volume discounts for Amazon EC2 and Amazon S3.

- **Main Features/Benefits**:
	- Central location to manage billing across all your AWS accounts.
	- Gain volume discounts for usage across all your AWS accounts.

<br>

## AWS Pricing Model
---

### AWS Pricing Model:

- AWS works on a **pay-as-you-go** mode, meaning you only pay for what you use when you are using it. There are no upfront cost, and charges immediately end when you stop using a particular service or feature (for the most part).
- No long-term contracts or complex licensing are required.
	- Exceptions can be something like reserved EC2 instances (not required)
- Volume discounts are available. So the more you use a service, the cheaper it can get (per unit used)
- There are no termination fees.
- AWS offers a "**Free Tier**" option for those new to AWS. Free Tier offers limited AS resources to you free of charge for 12 months (new accounts only).

### How Does AWS Pricing Work?

**Simple Storage Service (S3)**:
- **How much data** you store:
	- Applies to data at rest in S3
	- Charged per GB stored
	- Price per GB varies based on region and storage class
- **Request Pricing** - moving data in/out of S3:
	- PUT, POST, LIST, GET requests (API requests)
	- Lifecycle transition request
	- Data retrieval, data archive, data restore


**Elastic Cloud Compute (EC2):**
You are charged per second (based on an hourly rate) for the amount of time the instance is in a "running" state (applies to On-demand and Spot). Reserved instances are in one- or three year terms regardless of use. Hourly rates depend on options you select, such as:
- **The Purchasing Option** you choose:
	- On-demand, reserved, or spot
- **Instance Type** - the instance's processing capacity (think CPU):
	- Ex:  general purpose, compute optimized, GPU optimized, etc.
- **AMI Type** - think operation system:
	- Linux (price varies based on distro/software packages)
	- Windows (price varies based on version/software packages)
- **Region** the instance is provisioned in

<br>

## AWS Billing and Cost Tools
---

### What Is the TCO Calculator?

**Total Cost of Ownership (TCO) Calculator**
- The TCO calculator is a free tool provides by AWS that allows you to estimate the cost savings of using the AWS cloud vs. using an on-premise data center.
- By showing you how much you can save by using AWS, the calculator helps you reduce the Total Cost of Ownership (TCO) by avoiding large capital expenditures on I.T. hardware and infrastructure.
- The TCO Calculator can also provide directional guidance on cost savings.
- The TCO Calculator works by you inputting elements of your current or theoretical on-premises data center and comparing those cost requirements to how much it would cost in AWS.
- Elements can be added/modified as you move through the process to best estimate the cost savings.

### What Is the AWS Simple Calculator?

AWS Simple Calculator is used to estimate the anticipated AWS bill based on scenarios. Simple Calculator estimates your monthly bill and can provide a per-service breakdown of cost.

**AWS Simple Calculator** is being replaced by **AWS Pricing Calculator**, which estimates cost for AWS services based on use case.

The Pricing Calculator may be used to estimate cost using various workloads including on-demand and reserved instances. Pricing Calculator also helps you identify the cost-effective use case for your instance. Service costs may also be compared on a per-region basis. 

### What Is Cost Explorer?

- The Cost Explorer is a free tool that allows you to view charts of you costs.
- View cost data for the past 13 months.
- Forecast how much you are likely to spend over the newt twelve months.
- Use the explorer to discover patterns in how much you spend on AWS resources over time, and identify (cost) problem areas.
- Identify which services you use the most, as well as metrics like which Availability Zones have the most traffic or which linked AWS account is used the most.

<br>

## AWS Support Plans and Trusted Advisor
---

### AWS Account Support Plans

- Basic → Included with any AWS account
- Developer → Starts at $29 per month
- Business → Starts at $100 per month
- Enterprise → Starts at $15.000 per month

Although you get AWS support with each plan, the basic incentive to purchase a more expensive plan is the speed/availability in which you are given support. Enterprise plan holders will receive the highest priority for access to customer service and technical support.

### What Is AWS Trusted Advisor? (Simplified)

AWS Trusted Advisor is a service that "advises" and helps you optimize aspects of your AWS account.

### AWS Definition of Trusted Adviser

An online resource to help you reduce cost, increase performance, and improve security by optimizing your AWS environment. Trusted Advisor provides real-time guidance to help you provision your resources following AWS best practices.

**Trusted Advisor Categories:**
- Cost Optimization
- Performance
- Security
- Fault Tolerance

### Trusted Advisor Services:

- **Available to all AWS Support Plan Accounts:**
	- Security groups
	- IAM use
	- Is multi-factor authentication enabled on the root IAM user account?
	- EBS public snapshots
	- RDS public snapshots
	- Service limits
	- S3 Bucket Permissions
- **Available to Only Business and Enterprise Support Plan Accounts:**
	- Access to full list of Trusted Advisor checks
	- Notifications to stay up to data with weekly resource deployments
	- Programmatic access to retrieve/refresh Trusted Advisor results via API

<br>

## AWS Whitepapers and Documentation
---

### Whitepapers and Documentation:

**AWS Whitepapers** is a collection of technical documents that outline many AWS relevant topics, including (but not limited to):
- Architecture best practices
- Security best practices
- Cloud computing economics
- Serverless architecture

**AWS Service Documentation** is a collection of documents specific to each AWS service. They provide detailed technical explanations and walkthroughs on how to use each service and feature.

<br>

## AWS Billing and Support Services: Quiz (Correct answers only!)
---

- **Which of the following type of account receives only email access to Cloud Support Associates during business hours?**
	- Developer
- **Which of the following type of AWS account will receive support in less than 15 minutes when the support care is related to business-critical systems down?**
	- Enterprise
- **In regards to AWS Organizations, which of the following is true?**
	- AWS Organizations provides policy-based management for multiple AWS accounts.
- **In this scenario, we want to calculate our anticipated bill for resources we are about to create, which of the following tools can accomplish this task?**
	- AWS Simple Calculator
- **In this scenario, we want to consolidate billing between multiple AWS accounts. Which of these services would help us accomplish this goal?**
	- AWS Organizations
- **Which of the following is true about the AWS Pricing Model?**
	- AWS does not charge a termination fee.
- **Which of the following accurately describes the function of the AWS Cost Explorer?**
	- The AWS Cost Explorer is a free, easy to use tool that allows for viewing charts and usage history in order to manage AWS costs over time.
- **Which of the following types of AWS accounts have access to AWS Trusted Advisor? Please select the most appropriate answer.**
	- Basic, Developer, Business, and Enterprise
- **Which of the following types of AWS accounts have access to AWS Personal Health Dashboard? Please select the most appropriate answer.**
	- Basic, Developer, Business, and Enterprise
- **Which of the following statements is true?**
	- AWS Organizations is a service available to all AWS customers at no additional costs.
- **Which of the following AWS Tools will be replacing the AWS Simple Calculator?**
	- AWS Pricing Calculator
- **Which of the following describes the function of the TCO Calculator?**
	- The TCO Calculator is a free tool that allows for an estimation of the cost savings to be had by migrating to the AWS Cloud from an on-premises datacenter.
- **Which of the following is not one of the seven core checks performed by AWS Trusted Advisor?**
	- Unassociated Elastic IP Addresses
	- Amazon EC2 Reserved Instances Optimization
- **In this scenario, we want to control service usage across multiple AWS accounts using AWS Organizations. Which of the following would be used to accomplish this task?**
	- Service Control Policies
- **Which of the following guidelines should be followed if an AWS account is compromised?**
	- Change all IAM user passwords.
	- Respond to AWS through the AWS Support Center.
	- Change the AWS account root password.
	- Rotate and delete all API access keys.
	- Delete any resources that you do not remember creating.