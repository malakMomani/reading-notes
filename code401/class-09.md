# OAuth

**OAuth** : is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

**OAuth Component:**
`Client application` - The website or web application that wants to access the user's data.
`Resource owner` - The user whose data the client application wants to access.
`OAuth service provider` - The website or application that controls the user's data and access to it. They support OAuth by providing an API for interacting with both an authorization server and a resource server.

**Example** :
Step 1 – *The User Shows Intent*

**Joe (User)**: “Hey, Bitly, I would like you to be able to post links directly to my Twitter stream.”
**Bitly (Consumer)**: “Great! Let me go ask for permission.”

Step 2 – *The Consumer Gets Permission*

**Bitly**: “I have a user that would like me to post to his stream. Can I have a request token?”
**Twitter** (Service Provider): “Sure.  Here’s a token and a secret.”
The secret is used to prevent request forgery.  The consumer uses the secret to sign each request so that the service provider can verify it is actually coming from the consumer application.

Step 3 – *The User Is Redirected to the Service Provider*

**Bitly**: “OK, Joe.  I’m sending you over to Twitter so you can approve.  Take this token with you.”
**Joe**: “OK!”

`Bitly directs Joe to Twitter for authorization`

This is the scary part. If Bitly were super-shady Evil Co. it could pop up a window that looked like Twitter but was really phishing for your username and password.  Always be sure to verify that the URL you’re directed to is actually the service provider (Twitter, in this case).

Step 4 – *The User Gives Permission*

**Joe**: “Twitter, I’d like to authorize this request token that Bitly gave me.”
**Twitter**: “OK, just to be sure, you want to authorize Bitly to do X, Y, and Z with your Twitter account?”
**Joe**: “Yes!”
**Twitter**: “OK, you can go back to Bitly and tell them they have permission to use their request token.”
Twitter marks the request token as “good-to-go,” so when the consumer requests access, it will be accepted (so long as it’s signed using their shared secret).

Step 5 – *The Consumer Obtains an Access Token*

**Bitly**: “Twitter, can I exchange this request token for an access token?”
**Twitter**: “Sure.  Here’s your access token and secret.”

Step 6 – *The Consumer Accesses the Protected Resource*

**Bitly**: “I’d like to post this link to Joe’s stream.  Here’s my access token!”
**sa**: “Done!”

**The most common OAuth 2.0 grant types are listed below:**

- Authorization Code : used when the client wants to request access to protected resources on behalf of another user. This is the grant type most often associated with OAuth.

![explain](https://miro.medium.com/max/3000/1*m4CA9yzEuB2ctevS6OhA3w.png)

- Implicit : is a simplified flow that can be used by public clients, where the access token is returned immediately without an extra authorization code exchange step.

![explain](https://miro.medium.com/max/3000/1*ItytbOGAr-uS16ki5hQAkg.png)

- Password
- Client Credentials
- Device Code
- Refresh Token

**Pros:**

- Ease (يسهل) : A friend sends you a link to restaurant and you want to leave a comment. The only problem is that you’ve never been to this site before and don’t have an account. But due to OAuth you can easily get access through sign in using facebook/twitter/Google+ feature

- time saving in the long run.

- OAuth allows you to use one account to comment on several different sites.

- Privacy. You just found a bag you’d love to buy from an online store, but how do you know if you can trust them with your credit card? OAuth solves this

- Security. all OAuth data transfers must take place on SSL (Secure Sockets Layer) to ensure the most trusted cryptography industry protocols are being used to keep data as safe as possible.

- Control. Allows users to control when that timeframe window is up.

- Traffic. OAuth can allow things to be more casual.

**Cons:**

- Phishing (التصيد).
- Data misuse. (اساءه استخدام البيانات)

## TO REMEMBER

*Terminology*
► Access token — A token used to access protected resources.
► Authorization code — An intermediary token generated when a user authorizes a client to access protected resources on their behalf. The client receives this token and exchanges it for an access token.
► Authorization server — A server which issues access tokens after successfully authenticating a client and resource owner, and authorizing the request.
► Client — An application which accesses protected resources on behalf of the resource owner (such as a user). The client could be hosted on a server, desktop, mobile or other device.
►Grant — A grant is a method of acquiring an access token.
► Resource server — A server which sits in front of protected resources (for example “tweets”, users’ photos, or personal data) and is capable of accepting and responsing to protected resource requests using access tokens.
► Resource owner — The user who authorizes an application to access their account. The application’s access to the user’s account is limited to the “scope” of the authorization granted (e.g. read or write access).
► Scope — A permission.
► JWT — A JSON Web Token is a method for representing claims securely between two parties as defined in RFC 7519.
