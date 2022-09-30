# Chapter Sixteen: Other Noteworthy AWS Services

## Additional AWS Services
---

### Amazon Athena

Athena is a serverless interactive query service used to analyze data in Amazon S3 using standard SQL. Because Athena is serverless, there is no infrastructure to manage. Athena is billed only for queries that you run.


### Amazon EMR

Amazon EMR provides a managed Hadoop framework. Amazon EMR is designed for processing broad sets of big data, including log analysis, web indexing, machine learning, and financial analysis.


### Amazon Lightsail

Lightsail is a private virtual server (instance) aimed at developers to provide everything needed to launch a service or project quickly. There are number of "quick start" prepackaged setups to support a variety of operating systems and solutions.


### Amazon Rekognition

Amazon Rekognition provides video/image analysis. The service can identify objects, people, text, etc., in the image/video. Rekognition also support facial recognition and analysis.


### Amazon Device Farm (Mobile Lab)

Device Farm provides physical devices that can be used to test and troubleshoot applications on mobile devices, as well as help simulate real-world customer conditions.


### Amazon Mechanical Turk

Amazon Mechanical Turk (MTurk) is a crowdsourcing marketplace that simplifies outsourcing of processes and jobs to a distributed workspace. Practically any task that can be performed remotely (virtually) can be tasked via Mechanical Turk. Crowdsourcing is great for manual, time-consuming tasks that can be completed by distributed workers.

<br>

## Serverless Compute, Security and Compliance, and Additional Services: Quiz (Correct answers only!)
---

- **Which of these are allowed penetration testing without prior approval from AWS?**
	- RDS
	- EC2 instances
	- CloudFront
- **What AWS service will perform serverless computing?**
	- AWS Lambda
- **Which of the following services is not allowed penetration testing without prior approval?**
	- Amazon S3
- **Which of the following is not a use case for AWS Lambda?**
	- Data warehousing
- **What two services in combination, aid in DDoS mitigation?**
	- CloudFront and Route 53
- **In this scenario, we want a video/image analysis service for facial recognition purposes. Which of the following services can serve this purpose?**
	- AWS Rekognition
- **What is AWS Lightsail?**
	- One of AWS's VPS Services
- **In regards to the AWS Shared Responsibility Model, for which of these is AWS Responsible?**
	- CPU on physical hardware
	- Availability Zones
	- Host virtualization hardware
- **In what service could we use KMS to encrypt an object?**
	- S3
- **What is AWS Lambda?**
	- Compute service
- **Which of the following are options for creating Lambda functions? Please select the most appropriate answer.**
	- Author from scratch, using a blueprint, and browsing the serverless app repository
- **In regards to AWS KMS, which of these statements are true?**
	- Keys can be generated in a CloudHSM cluster.
	- Keys may be generated in KMS.
	- Keys may be imported from other encryption key services.
- **What service does AWS KMS integrate with for logging of key events?**
	- CloudTrail
- **What is Amazon Mechanical Turk used for?**
	- Crowdsourcing marketplace where you can outsource tasks.
- **In regards to penetration testing on AWS, which of these statements is true? Please select the most appropriate response.**
	- Limited penetration testing is allowed, but some require permission from AWS.
- **Which of the following services is a serverless interactive query service for analytics?**
	- Amazon Athena
- **In regards to security and compliance on AWS, what AWS service is a threat detection service that monitors for threats to AWS accounts and workloads?**
	- AWS GuardDuty
- **In this scenario, we want to enable notifications for KMS activity. What AWS service could be used with AWS KMS to send these notifications?**
	- SNS