# Bearer Authorization

- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Make a request to a third-party API endpoint
- Redirect to a third party authentication endpoint
- Make a request to the access token endpoint
- Receive access token
- Receive authorization code

---------------------------------------------

- most common usage is in credit card issues, because it's sensitive data, if I want to know if the user has sufficient credit available to authorize the transaction. 

`Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage`

- What’s a benefit of using OAuth instead of your own basic authentication? more strong and secure than the basic-auth

**TERMS** 

*Client ID* : is a public and unique identifier for apps

*Client Secret* : is a secret known only to the application and the authorization server.It must be sufficiently random to not be guessable

Authentication Endpoint
Access Token Endpoint
API Endpoint

*Authorization Code*: is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.

*Access Token*:are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage

## JWT : JSON WEB TOKEN

- is an open standard (RFC 7519) 
- Why it used : securely transfer info. between any two bodies(users , server)
- Digitally signed - info. is verified an trusted
- Compact : can send via URL , POST request ,HTTP header , fast transmission
- self-contained : contain info about the user, avoiding query the database more than once
- used for authentication / Information Exchange
- Header : {
  "alg":"HS256"
  "typ":"JWT"
}
- Payload : {
  "sub":"123456789",
  "name":"Malak",
  "admin": true
}
- Signature : HMACSHA256(base64UrlEncode(header) + "." + base64UrlEncode(payload), secret)
- JWT : header.payload.signature
- When should you use JSON Web Tokens?
  - Authorization
  - Information Exchange

- process: the browser will send post request to login , the server will generate JWT via Secret, then return the JWT to the browser, the browser will send the JWT again on the authorization header, server will JWT signature ang get the user info if it's match then will send the ewspone to the client