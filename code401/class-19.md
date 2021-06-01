# AWS: Events

**TERMS :**

**Serverless API:** architectures are application designs that incorporate third-party “Backend as a Service” (BaaS) services, and/or that include custom code run in managed, ephemeral containers on a “Functions as a Service” (FaaS) platform.

**Triggers:** is a Lambda resource or a resource in another service that you configure to invoke your function in response to lifecycle events, external requests, or on a schedule. Your function can have multiple triggers. ... Other AWS services and resources invoke your function directly.

**Dynamo vs Mongo** *DynamoDB* is a fully managed AWS service, *MongoDB* can be self installed or fully managed with *MongoDB* Atlas. ... *DynamoDB* uses tables, items and attributes, MongoDB uses JSON-like documents. *DynamoDB* supports limited data types and smaller item sizes; *MongoDB* supports more data types and has fewer size restrictions

-------------------------------------------------------------------------------------------

## SNS & SQS

**SNS** is a distributed publish-subscribe service.
**SQS** is distributed queuing service.

**SNS:**

- Simple Notification Service.
- is a web service that makes it easy to set up, operate, and send notifications from the cloud. It provides developers with a highly scalable, flexible, and cost-effective capability to publish messages from an application and immediately deliver them to subscribers or other applications. It is designed to make web-scale computing easier for developers.
- **How does Amazon SNS work?**
    It is very easy to get started with Amazon SNS. Developers must first create a “topic” which is an “access point” – identifying a specific subject or event type – for publishing messages and allowing clients to subscribe for notifications. Once a topic is created, the topic owner can set policies for it such as limiting who can publish messages or subscribe to notifications, or specifying which notification protocols will be supported (i.e. HTTP/HTTPS, email, SMS). Subscribers are clients interested in receiving notifications from topics of interest; they can subscribe to a topic or be subscribed by the topic owner. Subscribers specify the protocol and end-point (URL, email address, etc.) for notifications to be delivered. When publishers have information or updates to notify their subscribers about, they can publish a message to the topic – which immediately triggers Amazon SNS to deliver the message to all applicable subscribers.

**SQS:**

- Simple Queue Service.
- Amazon Simple Queue Service (SQS) and Amazon SNS are both messaging services within AWS, which provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates. Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components. Amazon SQS provides flexibility for distributed components of applications to send and receive messages without requiring each component to be concurrently available.

- A common pattern is to use SNS to publish messages to Amazon SQS queues to reliably send messages to one or many system components asynchronously.

![img](https://media.amazonwebservices.com/blog/sns_sqs_image_proc_2.png)
