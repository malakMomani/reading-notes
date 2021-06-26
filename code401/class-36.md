# Application State with Redux

1. **What are the advantages of storing tokens in “Cookies” vs “Local Storage”**
   - cookies: The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage. It's automatically sent in every HTTP request to your server.

   - local Storage : It's pure JavaScript and it's convenient. If you don't have a back-end and you're relying on a third-party API, you can't always ask them to set a specific cookie for your site.

2. **Explain 3rd party cookies.** is placed on a website by someone other than the owner (a third party) and collects user data for the third party. used for tracking for example

3. **How do pixel tags work?**
   - is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. Because it is so small, it can hardly be seen by visitors of a website or email recipients, it can hardly be seen by visitors of a website or email recipients.

   - The following data can be acquired and analyzed with a tracking pixel :
     - Operating system used (gives information on the use of mobile devices)
     - Type of website or email used, for example on mobile or desktop
     - Type of client used, for example a browser or mail program.
     - Client’s screen resolution
     - Time the email was read or website was visited
     - Activities on the website during a session (when using multiple tracking pixels)
     - IP address (gives information on the Internet Service Provider and location)

**Terms:**

**cookies :** are small blocks of data created by a web server while a user is browsing a website and placed on the user's computer or other device by the user’s web browser.

**authorization:**  is a security mechanism to determine access levels or user/client privileges related to system resources

**access control:** is a security technique that regulates who or what can view or use resources in a computing environment.

**conditional rendering:** is a piece of content that is displayed or rendered when a predefined condition is met.

----------------------------------------------------------------------------------------------------------------------------------

- Redux provides a solid, stable, and mature solution to managing state in your React application.
- Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized,