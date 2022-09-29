# Chapter Eleven: Monitoring and Logging

## CloudWatch (Monitoring, Metrics, and Logs)
---

### What Is CloudWatch? (Simplified)

CloudWatch is a service that allows you to **monitor** various elements of your AWS account.

### AWS Definition of CloudWatch

Amazon CloudWatch monitors your Amazon Web Services resources and the applications you run on AWS in real time. You can use CloudWatch to **collect and track metrics**, which are variables you can measure for your resources and applications. CloudWatch **alarms send notifications or automatically makes changes** to the resources you are monitoring **based on rules that you define**.

### CloudWatch Benefits:

- Monitor metrics for almost all your AWS resources
- Create and monitor custom metrics
- Create custom dashboards for easy viewing of metrics
- Monitor and store logs
- Set alarms and events (and trigger actions based on them)

<br>

## CloudTrail
---

### What Is CloudTrail? (Simplified)

CloudTrail allows you to monitor all actions taken by IAM users (ex: services accessed and actions taken - such as logging who deleted an S3 object).

### AWS Definition of CloudTrail

AWS CloudTrail is a service that enables **governance, compliance, operational, auditing, and risk auditing of your AWS account**. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. **CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services.** This event history simplifies security analysis, resource change tracking, and troubleshooting.