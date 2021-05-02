# Express

1. difference between **PUT** & **PATCH**
   - Put: HTTP method response for modifying resources where the user wants and will modifying the entire resource, For example, when you want to change the first name of a person in a database, you need to send the entire resource when making a PUT request.

   - PATCH: HTTP method response for modifying resourcess where the user wants and will modifying the part of the resource.

2. Insomnia, Postman, Stoplight.

| **   |      Swagger      |  APIDocs.js  |
|----------|:-------------:|------:|
| OK |  200 | 200 |
| Bad request |    400   |   400  |
| Authorization information is missing or invalid | 401 | - |
| not found. |   404   |   404  |
| Unexpected error. |   5XX   | - |
| forbidden |   -   |  403  |
| server error |   -   |  500  |

-> The difference between REST & SOAP

- REST : refer to Representational State Transfer , it's an architectural style that defines aset of recommendations for designing loosely coupled applications that use the HTTP protocol for data transmission.
- SOAP : refer to Simple Object Access Protocol , it's a standardlized protocol that sends messages using other protocols such as HTTP. It returns data to the receiver in XML format
- REST was created to address the problems of SOAP.

   | ** |      Swagger      |  APIDocs.js  |
   |----------|:-------------:|------:|
   | Meaning |  Simple Object Access Protocol | Representational State Transfer  |
   | Design |    Standardized protocol with pre-defined rules to follow.   |   Architectural style with loose guidelines and recommendations.  |
   | Approach | Function-driven (data available as services, e.g.: “getUser”) | Data-driven (data available as resources, e.g. “user”).  |
   | Statefulness |    Stateless by default, but it’s possible to make a SOAP API stateful.   |   Stateless (no server-side sessions).  |
   | Caching |    API calls cannot be cached.   |  API calls can be cached.  |
   | Security |    WS-Security with SSL support. Built-in ACID compliance.   |  Supports HTTPS and SSL.  |
   | Performance |   Requires more bandwidth and computing power.   |  Requires fewer resources.  |
   | Message format |   Only XML.   |   Plain text, HTML, XML, JSON, YAML, and others  |
   | Transfer protocol(s) |   HTTP, SMTP, UDP, and others.   |  Only HTTP  |
   | Recommended for |   Enterprise apps, high-security apps, distributed environment, financial services, payment gateways, telecommunication services.   |  Public APIs for web services, mobile services, social networks.  |
   | Advantages |   High security, standardized, extensibility.   |  Scalability, better performance, browser-friendliness, flexibility.  |
   | Disadvantages |   Poorer performance, more complexity, less flexibility.   |  Scalability, better performance, Less security, not suitable for distributed environments.  |

**Web Server** :  is software and hardware that uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the World Wide Web.

**Express** : is a free and open-source web application framework for Node. js. It is used for designing and building web applications quickly and easily. Web applications are web apps that you can run on a web browser.

**Routing** : is a mechanism where HTTP requests are routed to the code that handles them. To put simply, in the Router you determine what should happen when a user visits a certain page.

**WRRC** : Web Request Response Cycle
