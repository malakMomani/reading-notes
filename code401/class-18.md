# AWS: API, Dynamo and Lambda

1. **What are serverless functions?**
   is a software design pattern where applications are hosted by a third-party service, eliminating the need for server software and hardware management by the developer. like *AWS Lambda*

2. **If you were to create a system that emulated Lambda functions, how would you do it?**

3. **Describe how a CDN works**
   - The goal of the CDN is to reduce latency by reducing the physical distance that the request has to travel.
   - CDNs store a cached version of your website content in multiple geographical locations around the world,
   - These Location called PoPs (points of presence)
   - The PoPs contain their own caching servers and will be responsible for delivering that content in the user’s location.
   - when the uswe request a web page will search about this page in the caching servers that near from th user regoin
   - if CDN didn't find the apporopriate response will retriwve from original server and save this new request into its cahe

**TERMS:**

- **Serverless Functions** : is a cloud computing execution model in which the cloud provider allocates machine resources on demand, taking care of the servers on behalf of their customers

- **Cloud Storage**:  is a way for businesses and consumers to save data securely online so that it can be accessed anytime from any location and easily shared with those who are granted permission.

- **CDN** :  is a geographically distributed network of proxy servers and their data centers. The goal is to provide high availability and performance by distributing the service spatially relative to end users.

-------------------------------------------------------------------------------------------------------------

## Amazon API Gateway

> is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

**How does API Gateway work?**

- API Gateway sits between the backend services of your API and your API’s users
- Handling the HTTP requests to your API endpoints and routing them to the correct backends.
- It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services.
- It can also generate API references from your definitions and make them available to your users as API documentation.
- Many AWS services support integration with Amazon API Gateway, including:
  - **AWS Lambda**: run Lambda functions to generate HTTP API responses.
  - **AWS SNS**: publish SNS notifications when an HTTP API endpoint is accessed.
  - **Amazon Cognito**: provide authentication and authorization for your HTTP APIs.

-------------------------------------------------------------------------------------------------------------

## DynamoDB

> is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

- reliable performance even as it scales;
- a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
- a small, simple API allowing for simple key-value access as well as more advanced query patterns.

**use cases:**

- Applications with large amounts of data and strict latency requirements
- Serverless applications using AWS Lambda.
- Data sets with simple, known access patterns.
