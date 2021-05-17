# Access Control (ACL)

1. When is Basic Authorization used vs. Bearer Authorization?
   - Basic Authorization: to login and sign up / user accounts
   - Bearer Authorization: after authenticating user to authorize him in the website.
2. What does the JSON Web Token package do?
   - create access tokens
3. What considerations should we make when creating and storing a SECRET?
   - store it safely by encrypt it in .git repo
   - use it withv enviroment variables

## TERMS

*encryption* : is the process of scrambling or enciphering data so it can be read only by someone with the means to return it to its original state.

*token* : it's a string used to authorize the user in the system

*bearer* : it's a token created for you by the Authentication server. When a user authenticates your application (client) the authentication server then goes and generates for you a Token

*secret*: message send with a token to make it more secure

*JSON Web Token*: is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

--------------------------------------------------------------------

## Role-Based Access Control(RBAC)

User => Role => Rights

- in the systems there is many roles , like user , admin and guest for example
- each role accessing some functionality in the system
- access rights associated with roles
- users authenticate themselves to the system

**Benefits** :

- Policy need not be updated when a certain person with a role leaves the organization
- new user should be able to activate the desire role
- Revisiting least privilege
- user in one role ha accesss to subsets of the files

`RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.`

**Access control lists (ACL)** — An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.  As a simple example, an ACL could be used to allow users from one department to make changes to a document, while only allowing users from other departments to read the document.

**Attribute-based access control (ABAC)**, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.

### Steps to create RBAC

1. Inventory your systems : list the things that want to add roles on it.
2. nalyze your workforce and create roles: group these things into roles with common access needs.
3. Assign people to roles'
4. Never make one-off changes
5. Audit: review your roles, and the access permitted for each