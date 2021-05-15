# Authentication

**Explain what a “Singleton” is (in Computer Science terms)**: is a class that allows to instantiate only one object of itself and give access to that instance, This helpful when my system needs only one object to coordinate actions across my system. A single object used across systems remains constant and needs to be defined only once rather than many times.

**Explain how the Singleton pattern can be used with Node modules, specifically with classes**: for Example if I want to save every log in the system, I can make the object do the log rather than console.log(), and inside it, I can save the time and the text of the log. That object must be the same and must use in all modules in my program, so must make it singleton and return the only instance at any time the user will use it.

**If you were tasked with building a middleware system as Express uses, what approach might you take to construct/operate it?**:
modularity

--------------------------------------------------------------------------
**Router Middleware**: the way to define the routes of middlewares and which routes should be handled by that middleware

**Dynamic Module Loading**: dynamically load modules only when they are needed, rather than having to load everything upfront. Using the `import()` method and passing to it the path of the module, it will return a promise with a module object giving you access to that object, Example:

```
import('./modules/myModule.js')
  .then((module) => {
    // Do something with the module.
  });
```

**Singleton Pattern**: is a class that allows to instantiate only one object of itself and give access to that instance
**CRUD -> REST Method Matches**:

| CRUD      | REST |
| ----------- | ----------- |
| CREATE      | POST       |
| READ   | GET        |
| UPDATE   | PUT        |
| DELETE   | DELETE        |

**Mock Testing**: using jest dependency, mocks provide us with the capability to stub the functionality provided by a dependency and a means to observe how our code interacts with the dependency. Mocks are especially useful when it's expensive or impractical to include a dependency directly into our tests, for example, in cases where your code is making HTTP calls to an API or interacting with the database layer.

--------------------------------------------------------------------------

## Securing Passwords with Bcrypt Hashing Function

- In all web services we need to store user data in the database, including passwords
- we don't store these passwords in the database as plaintext, we have to encrypt it, if any attacker steal the database he can't see the actual plaintext password
- Hash algorithm is the most common way to encrypt passwords, but it has some weaknesses.
- Brute Force attack: Hashed can't be reversed, but the attacker can keep trying valued until he get the same hash value.
- Hash Collision attack
- Solve the weakness : BCrypt, IT's SLOW AND STRONG AS HELL
- BCrypt: make the brute force attacks slower and minimize the impact, based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor, different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks

--------------------------------------------------------------------------

## Basic access authentication

is a method for an HTTP user agent to provide a user name and password when making a request.

- **Authentication** : is the process of verifying that an individual, entity or website is whom it claims to be,by submitting a username or ID and one or more items of private information that only a given user should know.
- **Session Management** is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction

- Do NOT allow login with sensitive accounts (i.e. accounts that can be used internally within the solution such as to a back-end / middle-ware / DB) to any front-end user-interface
- Do NOT use the same authentication solution (e.g. IDP / AD) used internally for unsecured access (e.g. public access / DMZ)

- Minimum length of the passwords should be enforced by the application. Passwords shorter than 8 characters are considered to be weak
- Maximum password length should not be set too low, as it will prevent users from creating passphrases
- do not silently truncate passwords
- Allow usage of all characters including unicode and whitespace. There should be no password composition rules limiting the type of characters permitted.
- Ensure credential rotation when a password leak, or at the time of compromise identification.
- Include password strength meter to help users create a more complex password and block common and previously breached passwords
- Store Passwords in a Secure Fashion
- Compare Password Hashes Using Safe Functions
- Require Re-authentication for Sensitive Features
