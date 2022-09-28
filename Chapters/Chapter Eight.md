# Chapter Eight: AWS Storage Services

## Overview of AWS Storage Services
---

### What Is Simple Storage Service (S3)? (Simplified)

An online, bulk storage service you can access from almost any device.

### AWS Definition of S3

Amazon S3 has a simple web services interface that you can use to **store and retrieve any amount of data, at any time, from anywhere on the web**. It gives any users access to the same highly scalable, reliable, fast, inexpensive data storage infrastructure that Amazon uses to run its own global network of websites. The service aims to maximize benefits of scale and to pass those benefits on to users.

### Components and Structure:

- **Basics**:
	- S3 = Simple Storage Service
	- It is AWS's primary storage service
	- You can store any type of file in S3
- **Buckets**:
	- Root-level "folders" you create in S3 are referred to as **buckets**.
	- Any "subfolder" you create in a bucket is referred to as a **folder**.
- **Objects**:
	- Files stored in a bucket are referred to as **objects**.
- **Regions**:
	- When you create a bucket, you must select a specific region for it to exist in. This means **any data you upload to the S3 bucket will be physically located in a data center in that region**.
	- **Best practice** is to select the region that is physically **closest to you** (to **reduce transfer latency**)
        - **OR**
	- If you are serving files to a **customer** based in a certain area of the world, **create the bucket in a region closest to you customers** (to reduce latency for your customers)

<br>

## S3 Storage Classes
---

A **storage class** represents the "classification" assigned to each object in S3.

**Available storage classes include:**
- Standard
- Standard-IA (Infrequent Access)
- One-Zone-IA (Infrequent Access)
- Intelligent-Tiering
- Glacier
- Glacier Deep Archive

Each **storage class** has varying attributes that dictate things like:
- Storage Cost
- Object **Availability**
- Object **Durability**
- Frequency of Access (to the object)

Each object must be assigned a storage class ("Standard" is the default class)
You can change the **storage class** of an object at any time (**for the most part**)

### Other S3 Features and Benefits

- **Features**
	- **Object Sharing**:
		- The ability to make any object publicly available via an URL link.
	- **Object Lifecycles**:
		- Set rules to automatically transfer objects between storage classes at defined time intervals.
	- **Object Versioning**:
		- Automatically keep multiple versions of an object (when enabled).
- **Benefits**
	- Durable, reliable, scalable
	- Security (offers three different kinds of encryption)
	- Integrates with almost all other AWS services
	- Can run big data analytics on objects directly in S3
	- Easy to get data in and out of S3
	- Robust admin and access management options available

<br>

## Storage Gateway
---

### What Is a Storage Gateway?

A way to integrate your existing application services with AWS cloud storage services without fully migrating to the AWS cloud. Applications connect to the AWS cloud using a virtual server or hardware device using common storage protocols. Data can be backed up to the AWS cloud, or the data may be moved to the AWS cloud and cached locally at your data center. All data that is transferred using Storage Gateway is optimized for fast and efficient transfer.

### Storage Gateway Deployment Types

- **File Gateway**
	- Data is uploaded to S3 for use with object-based workloads. S3 file storage can also be used for storage tiering to allow for data storage on the most cost-effective storage class.
- **Volume Gateway**
	- Volumes are created in the AWS cloud. The applications in the customer data center can access these volumes. There are two types: stored volumes and cached volumes. With **stored volumes**, all data is stored at the customers location (data center) and periodically backed up to AWS using snapshots. **Cached volumes** store the data in the AWS cloud, and the data is cached in the customer's data center for fast access.
- **Tape Gateway**
	- Cost-effective, long-term, off-site data archiving. A virtual tape library (VTL) interfaces with the customer's existing tape backup software.

<br>

## AWS Storage Services: Just the FAQs
---

- AWS Simple Storage Service (S3)  is a bulk storage service.
- Buckets are the equivalent of top-level folders. Subfolders may also be created. Objects may be uploaded into folders or directly into a bucket.
- S3 storage classes include:
	- **Standard**
	- **Standard-IA**
	- **Intelligent-Tiering**
	- **One Zone-IA**
	- **Glacier**
	- **Glacier Deep Archive**
- Storage classes define durability and availability ratings, as well as minimum storage duration (billing).
- View the following chart for more information on S3 durability and availability: https://aws.amazon.com/s3/storage-classes/
- Storage Gateway provides a hybrid environment for storing data between the customer site and AWS cloud. "Storage Gateway is a highly optimized data transfer mechanism, with bandwidth management, automated network resilience, and efficient data transfer".
- There are three Storage Gateway types:
	- File Gateway
	- Volume Gateway
	- Tape Gateway

<br>

## AWS Storage Services: Quiz (Correct answers only!)
---

- **A hospital organization wants to store patient health information as cheap as possible for archive purposes and is not worried about retrieval periods. What would be the most appropriate and cost-effective storage class for this case?**
	- Glacier Deep Archive
- **Which of these are examples of cloud bulk storage?**
	- Amazon S3
	- Google Drive
	- Dropbox
- **What S3 term is used in place of "file"?**
	- Object
- **What is S3?**
	- Storage Service
- **S3 is an example of _____.**
	- Bulk Storage
- **Which of the following is an example of block storage?**
	- Amazon EBS
- **What is the root level folder you create in S3 called?**
	- Bucket
- **What S3 storage class is the most expensive?**
	- Standard