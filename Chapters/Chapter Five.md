# Chapter Five: IAM: Managing Users, Groups, and Roles

## Overview of Identity and Access Management: Part 1
---

### What is IAM?

- **IAM** (**I**dentity  and **A**ccess **M**anagement) is the service where AWS user accounts and their access to various AWS services is managed.
- The common use of IAM is to manage:
	- Users
	- Groups
	- Access Policies
	- Roles
	- User Credentials
	- User Password Policies
	- Multi-Factor Authentication (MFA)
	- API keys for programmatic (CLI) access
- The user created when you create an AWS account is called the **root** user.
- By default, the root user has full administrator rights and access to every part of the account
- Any new or additional users created in the AWS account are created with no access to any AWS resources. The only granted access is the ability to login.
- For a user to access  an AWS service, permission must be granted to that user, which is managed in/by IAM

### IAM Best Practices

- **AWS Best Practices:**  Guidelines that recommend settings, configurations, and architecture for maintaining a high level of security, accessibility and efficiency.
- When a new AWS root account is created, it is best practice to complete the tasks listed in IAM under **Security Status**, including:
	- **Delete** your root access keys
	- **Activate** MFA on your root account
	- **Create** individual IAM users
	- **Use groups** to assign permissions
	- **Apply** an IAM password policy

<br>

## Overview of Identity and Access Management: Part 2
---

### What is MFA?

- MFA stands for **M**ulti-**F**actor **A**uthentication.
- It is an additional layer of security on your root account that is provided by a third party.
- It provides a continually changing, random, six-digit code you need to input (along with your password) when logging in to your root account

### How do you get an MFA code?

- **Virtual MFA Device**
	- Smartphone or tablet
	- Commonly used app (IOS and Android): Google Authenticator
- **Hardware key fob**
	- Small physical device with a display that you can attach to your keychain
	- Ordered directly from AWS
- **API keys for programmatic (CLI) access**
	- Special credentials required for accessing AWS resources via the command line interface (CLI)

![Image](./images/mfa.png)

### Best Practices for IAM Users:

- Best practice is to **never** use your root account for day-to-day use.
- If you want full admin access, create an IAM user and attach the **AdministratorAccess** policy to it.
- Use that account as your daily driver

### Best Practices for IAM Groups

- An IAM group is a collection of IAM users. Groups allow you to set and manage permissions for multiple users at the same time.
- Groups are a more convenient and efficient way to manage account permissions.

### Best Practices for IAM Password Policy

- A password policy dictates the format and expiration rules that a user must follow when creating or modifying their password.
- These rules include:
	- Length requirements
	- Case requirements
	- Number requirements
	- Non-alphanumeric requirements
	- Password expiration
	- Password reuse
	- User rights to change their own password
	- Administrator reset requirements

<br>

## IAM User, Groups, Roles, and Policies
---

### IAM Users

- **IAM users** are individuals who have been granted access to an AWS account.
- Each IAM user has three main components:
	- A **username**
	- A **password**
	- Permissions to access various AWS services
- Without permissions being explicitly  granted to an IAM user, that user will not be able to  access any AWS services.
- Generally, a company's IT department will be responsible for "attaching" what are called **IAM permission policies** to an IAM user based on what that user needs access to (in order to do their job).

<br>

## IAM: Just the FAQs (Summary)
---

- The **root user** account is created when the AWS account is created.
- The root account has access to **everything** within the AWS account.
- The root account should **not** be used for daily management tasks.
- Create an additional account for **daily administration**.
- **IAM users** have no rights by default when created, except the ability to login.
- **IAM groups** can be used to grant multiple users the same access.
- **Policies** assigned to users and groups grant access to AWS resources.
- **IAM roles** are used to grant one AWS resource access to another resource (ex: allow EC2 to access S3).
- **Multi-Factor Authentication (MFA)** provides an additional layer of protection when logging in to AWS.
- Use **password policies** to enforce password complexity and strength.
- **API access keys** may be used for logging in to the command line interface.

<br>

## IAM: Managing Users, Groups, and Roles (Quiz / Correct answers only!)
---

- **Which AWS managed policy could be attached to an IAM User to grant all access permissions?**
	- AdministratorAccess
- **What access privileges does a new IAM user have by default?**
	- AWS Console login access
- **In this scenario, we have an IAM User with an AWSDenyAll policy, but this user is also in an IAM Group with access to various AWS services. These services include S3, EC2, VPC, and IAM. Which of the following resources can this user access?**
	- The IAM user cannot access any of the AWS services
- **Which of the following is IAM commonly used to manage?**
	- Users & Groups
	- API access keys
	- Access Policies
	- Password Policies
- **An EC2 instance needs to access S3. What is the most appropriate way to provide the EC2 instance access to S3?**
	- IAM Role
- **Which of the following is not a method of getting or using MFA codes?**
	- Single sign-on