# Data Modeling

1. Name 3 advantages to Test Driven Development
   - high code quality. ...
   - Detailed project documentation. ...
   - TDD reduces the time required for project development. ...
   - Code flexibility and easier maintenance. ...
   - With TDD you will get a reliable solution. ...
   - Save project costs in the long run.
2. n what case would you need to use `beforeEach()` or `afterEach()` in a test suite?
   when we use jest test package and we want to spy on some method if it's called or not
3. What is one downside of Test Driven Development
   writting the test code is taking time
4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
   it's the inheritence proprety in the classes that very usefull
5. Why REST?
   stateless server, responds in different formats such as XML and JSON , easy way of dealing with requests, each request responds individually and flexibility of it, it can easy modified, answers many clients who can ask for different data types.

**functional programming**: The way of thinking about software construction it empazies on declartions and creating functions rather than excuting.

**object-oriented programming (OOP)** : programming model based on object concept, which have properties and behaviour.

**class** : code template for creating objects.

- `super` : base class , parent class , super class
- `this` : refer current class instance object

**Test Driven Development (TDD)** :  is a process of modifying the code in order to pass a test designed previously. includes refactoring a code i.e. changing/adding some amount of code to the existing code without affecting the behavior of the code.

**Jest** : is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase

**Continuous Integration (CI)** : is the practice of automating the integration of code changes from multiple contributors into a single software project

**REST** : is a software architectural style which uses a subset of HTTP. It is commonly used to create interactive applications that use Web services. A Web service that follows these guidelines is called RESTful

**Data Model** :  is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.

-----------------------------------------

## SQL vs NoSQL

| SQL  | NoSQl |
| ------------- | ------------- |
| Relational Databases (RDBMS)  | non-relational or distributed database.  |
| table based  |document based, key-value pairs, graph databases or wide-column stores.  |
| have predefined schema  | have dynamic schema for unstructured data |
| vertically scalable  | horizontally scalable |
| uses SQL ( structured query language )  | The syntax of using UnQL varies from database to database. |
|  example : Postgres   | example : MongoDB |
| complex queries: SQL databases are good  | s NoSQL databases are not good |
| For the type of data to be stored: SQL databases are not best fit for hierarchical data storage  | NoSQL database fits better for the hierarchical data storage |
| You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server  | You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic. |
| SQbest fit for heavy duty transactional type applicationsL  | it is still not comparable and sable enough in high load and for complex transactional applications. |
| Excellent support are available for all SQL database from their vendors.  | you still have to rely on community support |
| SQL databases emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability)   | NoSQL database follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance ) |

**Mongo DB** :  is one of the most popular document based NoSQL database as it stores data in JSON like documents. It is non-relational database with dynamic schema.

- MongoDB benefits and strengths: speed , scalability, Manageable, Dynamic Schema.
