# Chapter Thirteen: SQL and NoSQL

## Relational Database Services (RDS) and DynamoDB
---

### AWS Primary Database Options:

- **Relational databases** known as "**SQL**"
	- Amazon offers **RDS**
- **Non-relational databases** known as "**NoSQL**"
	- Amazon offers **DynamoDB**


### What is RDS? (Simplified)

Relational Database Service is a **SQL database service** that provides a wide range of SQL database options to select from.
- **SQL Options Include:**
	- Amazon Aurora
	- MySQL
	- MariaDB
	- PostgreSQL
	- Oracle
	- Microsoft SQL Server

### AWS Definition of RDS

Amazon Relational Database Service is a web service that makes it easier to set up, operate, and scale a relational database in the cloud. It provides **cost-efficient, re-sizable capacity** while automating time-consuming administration tasks such as hardware provisioning, database setup, patching,  and backups. It frees you to focus on your applications so you can give them the fast performance, high availability, security and compatibility they need.

### What Is DynamoDB? (Simplified)

DynamoDB is a **NoSQL database service**. Unlike RDS, DynamoDB does **not** provide other NoSQL software options.
- **DynamoDB can replace (or is very similar to):**
	- MongoDB
	- Cassandra DB
	- Oracle NoSQL


### AWS Definition of DynamoDB

Amazon DynamoDB is a fast and flexible **NoSQL database service** for all applications that need **consistent, single-digit millisecond latency at any scale.** It is a fully managed cloud database and supports both document and key-value store models. Its flexible data model, reliable performance, and automatic scaling of throughput capacity makes it a great fit for mobile,  web, gaming, ad tech, IoT, and many other applications.

### To SQL or to NoSQL?

What is the difference?

- **Amazon RDS**:
	- Stores related data is tables (using columns and rows)
	- Typically used for very structured data, such as contact lists
- **Amazon DynamoDB**:
	- Stores related data in JSON-like, name-value documents
	- Typically used for non-structured data such as cataloging documents


### What Are the Differences/Benefits?

- **RDS**:
	- For when you need a SQL database option
	- Easy to set up, highly available, fault-tolerant, and scalable
	- Used when data is clearly defined
	- Common use cases include online stores and banking systems
- **DynamoDB**:
	- For when you need a NoSQL database option
	- Fast,  highly scalable, and fully managed
	- Used when data is fluid and can change
	- Common use cases include social networks, web analytics

<br>

## ElastiCache and Redshift
---

### What Is ElastiCache? (Simplified)

ElastiCache is a data caching service used to help improve speed/performance of web applications running on AWS.


### AWS Definition of ElastiCache

Amazon ElastiCache is a web service that makes it easy to deploy, operate, and scale an in-memory data store or cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, secure in-memory data stores, instead of relying entirely on slower disk-based databases. Amazon ElastiCache supports two open-source in-memory engines.
- **Redis**: A fast, open source, in-memory data store and cache
- **Memcached**: A widely adopted memory object caching system

### What Is Redshift? (Simplified)

Redshift is a **data warehouse** database service designed to handle **petabytes** of data for analysis.

### AWS Definition of Redshift

Amazon Redshift is a fast, **fully managed data warehouse** that makes it simple and cost-effective to analyze all your data using standard SQL and your existing Business Intelligence (BI) tools. It allows you to **run complex analytic queries against petabytes of structured data**, using sophisticated query optimization, columnar storage on high-performance local disks, and massively parallel query execution.

<br>

## Databases: Just the FAQs (Summary)
---

- **RDS**
	- RDS stands for Relational Database Service.
	- RDS is a SQL database service.
	- SQL options include Amazon Aurora, MySQL, MariaDB, PostgreSQL, Oracle, and Microsoft SQL Server.
	- RDS stores related data in tables using columns and rows.
	- RDS is typically used for very structured data, such as contact list.
- **DynamoDB**
	- DynamoDB is a NoSQL database service.
	- DynamoDB can replace (or is similar to) MongoDB,  Cassandra DB, and Oracle NoSQL.
	- Supports documents and key-value store models.
	- DynamoDB is a great fit for mobile, web, gaming, ad tech, and IoT.
	- Designed for applications that need consistent, single-digit millisecond latency at any scale.
	- DynamoDB stores related data in JSON-like, name-value documents.
	- Typically used for non-structured data, such as cataloging documents.
- **Redshift**
	- Redshift is a fully managed data warehouse database service designed to analyze data using standard SQL and Business Intelligence (BI) tools.
- **ElastiCache**
	- Amazon ElastiCache is a web service that makes it easy to deploy, operate, and scale an in-memory data store or cache in the cloud.

<br>

## SQL and NoSQL: Quiz (Correct answers only!)
---

- **Which of the listed statements are true?**
	- Amazon RDS does support alternative database software options.
	- Amazon RDS is a SQL database service.
	- Amazon DynamoDB is a NoSQL database service.
- **Which of these AWS services is best suited for analyzing data using standard SQL and Business Intelligence(BI) tools?**
	- Amazon Redshift
- **Which of the following is not a SQL database engine?**
	- DynamoDB
- **Which of the following is a non-relational database service provided by AWS?**
	- DynamoDB
- **Which of these are relational database engines supported by Amazon RDS?**
	- MySQL
	- MySQL
	- PostgreSQL
- **Which database service uses a JSON document and key-value store model?**
	- Amazon DynamoDB
- **Which of the listed answers are the benefits of Amazon RDS?**
	- Fully-managed
	- Cost-Efficient
	- Scalable
	- Resizable Database
- **Which of the following NoSQL databases does Amazon DynamoDB replace?**
	- MongoDB
	- Cassandra DB
	- Oracle NoSQL
- **What is Amazon RDS?**
	- A Relational Database Service
- **What is Elasticache?**
	- A data caching database service