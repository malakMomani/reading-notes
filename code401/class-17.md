# AWS: S3 and Lambda

1. **Describe “The Cloud”**
   - servers that are accessed over the Internet, along with the software and databases that run on those servers, enables users to access the same files and applications from almost any device
   ![cloud](https://www.guru99.com/images/1/031519_0703_Advantagesa1.png)

2. **What is a container (as it relates to computers and servers)?**
   - is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

3. **What is auto-scaling?**
   - increase the infrastructure or any service that your app need automatically using aws

4. **What is bandwidth?**
   - The maximum amount of data transmitted over an internet connection in a given amount of time.
   - Bandwith vs Speed ==> Bandwith how much information you receive every second, while speed is how fast that information is received or downloaded
   - Bandwidth vs latency ==> bandwidth is the amount of information sent per second, latency is the amount of time it takes that information to get from its source to you.
   - Bandwidth vs throughput ==> bandwidth is the max amount of data, throughput is how much of that data makes it to its destination – taking latency, network speed, packet loss and other factors into account.

**TERMS:**

**Server Instances :** is a collection of SQL Server databases which are run by a solitary SQL Server service or instance

**Containers:** are packages of software that contain all of the necessary elements to run in any environment. In this way, containers virtualize the operating system and run anywhere, from a private data center to the public cloud or even on a developer's personal laptop.

**Cloud Services:** wide range of services delivered on demand to companies and customers over the internet

**Cloud Architecture :** refers to the various building components that make up a cloud

**AWS :** is the world's most comprehensive and broadly adopted cloud platform, offering over 200 fully-featured services from data centers globally

------------------------------------------------------------------------

## Amazon S3

> is an object storage service that offers industry-leading scalability, data availability, security, and performance , can use it to store and protect any amount of data for a range of use cases

**Benifits:**

- Industry-leading performance, scalability, availability, and durability(قوة التحمل).

- Wide range of cost-effective storage classes
  - **S3 Storage Classes** - support different data access levels at corresponding rates
  - **S3 Storage Class Analysis** - discover data that should move to a lower-cost storage class based on access patterns
  - **S3 Lifecycle** - configure its policy to execute the transfer.
  - **S3 Intelligent-Tiering** - store data with changing or unknown access patterns in it , which tiers objects based on changing access patterns and automatically delivers cost savings.
  - **S3 Outposts** storage class, you can meet data residency requirements, and store data on-premises in your Outposts environment using S3 on Outposts.

- Unmatched security, compliance, and audit capabilities

- Easily manage data and access controls

- Query-in-place and process on-request
  - Use **Amazon Athena** to query S3 data with standard SQL expressions
  - **Amazon Redshift** Spectrum to analyze data that is stored across your AWS data warehouses and S3 resources.
  - **S3 Select** to retrieve subsets of object data, instead of the entire object

- Most supported cloud storage service

**Use Cases:**

- Backup and restore
- Disaster recovery (DR)
- Archive
- Data lakes and big data analytics
- Hybrid cloud storage
- Cloud-native applications

### AWS Lambda

> is one of the most popular serverless computing services out there. It is also the most popular provider used with the Serverless Framework

- The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

- “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

- Lambda can save you time on operational tasks. When there is no infrastructure to maintain, you can spend more time working on the application code—

**Benifits :**

- No servers to manage
- Continuous scaling
- Cost optimized with millisecond metering
- Consistent performance at any scale

> Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.
