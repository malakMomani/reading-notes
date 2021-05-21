# Event Driven Applications

1. Why is access control important?
    limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.

2. Describe an application that would need access control.
   social media account, first of all it will need to authenticate by username and password, the user can login and access the parts that he authorize to access using access token

3. What is a role used for? to determine what part of the system this client has access to it.

**TERMS:**

*Authorization:* is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features. This is the process of granting or denying access to a network resource which allows the user access to various resources based on the user's identity.

*Role Based Access Control:* is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

*Capabilities:* list of actions that user can be able to do it.

---------------------------------------------------------------------------------------

## Event-Driven Programming in Node.js

**What is Event-Driven Programming?**
> is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision

Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.
- Emitters :

---------------------------------------------------------------------------------------

- events module from node.js.
- `npm i events`

```
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

- The EventEmitter class is defined and exposed by the events module
