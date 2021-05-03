# Readings: Express REST API

1. Name 3 real world use cases where you’d want to change the request with custom middleware :
   - log in authentication
   - in chat app sending and recieving messaging
   - API security
2. True or false: The route handler is middleware?
   - **false** the middleware is a part of code to preparing the handler
3. In what ways can a middleware function end the process and send data to the browser?
   - when invoked the `next()` with no argument
4. At what point in the request lifecycle can you “inject” middleware?
   - at the beginning of the handler function ,before it do its' work.
5. What can cause express to error with “Request headers sent twice, cannot start a second response”
   - when handle the same route with the same method.

-----------------------------------------------------------
**Middleware** : function comes in the middle of req and res that prepare the handler of the routes take req and res objects with the next function as parameters
**Request Object** : represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
**Response Object** : represents the HTTP response that an Express app sends when it gets an HTTP request.
**Application Middleware** : software that have common middlewares serviced which used in the applications
**Routing Middleware** : the way to define the routes of middlewares and which routes should be handling by that middleware
**Test Driven Development** : (TDD) : is software development that based on test unites of the parts of code to validate what the code will do
**Behavioral Testing** :  (BDD) is a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests.

-----------------------------------------------------------

## Classes

> is an template for creating objects , it has attributes(proprieties) and methods(behavior). it's a special type of functions

The class can define by :

- Class declarations :

  ```
  class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  }
  ```

- Class expressions :

  ```
  let Rectangle = class {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  };
  ```

Sub classing with `extends` : The `extends` keyword is used in class declarations or class expressions to create a class as a child of another class.

## Express Routing

- **Routing** : mechanisim to define the end points in the server and specify how to the server will respond
  ex: `app.get('/item');`
- route methods is : get , post
- **Route paths**: in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.
- **Route parameters** : specify after `:` notation, ex. `app.post('/books/:bookId');`
- `app.route()` : to add deferent methods to the same route with different handlers
