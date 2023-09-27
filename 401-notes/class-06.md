# Class 06 Notes

## Readings

### Securing Passwords

Explain to a non-technical friend how you would safely hash and store a password.

- Imagine your password is like a secret code that only you should know. To keep it safe, we don't store the actual password. Instead, we use a special tool called a "hasher" to turn it into a secret recipe that's impossible to turn back into the original password.

What is Bcrypt?

- It is a cryptographic hashing function and a password hashing library commonly used in web development and security applications. It's specifically designed for securely storing passwords.

Why might you use something like Bcrypt?

- For password security, hashing and storing.

### Basic Auth

What is Basic Authentication?

- It is a simple authentication scheme used in HTTP (Hypertext Transfer Protocol) where a user's credentials, typically a username and password, are sent as part of an HTTP request. It's a basic and widely supported method for verifying a user's identity when accessing a web application or API.

What properties are necessary in the header of a Basic Auth request?

- An authorization header that includes this string.

Authorization: Basic base64(username:password)

How are username:password in Basic Auth encoded?

- Using the base64 encoding method

### OWASP auth cheatsheet

Define the authentication process to a non-technical recruiter.

- Imagine you have a secret club, and you need to make sure only the right people can enter. Authentication is like the bouncer at the club's entrance. It's a process to verify if someone is who they claim to be.

How should your error messaging respond (both HTTP and HTML)? Why?

- HTTP Response Codes: When something goes wrong during authentication, the server should respond with the appropriate HTTP status code. Common codes include:

200 OK: When authentication is successful.
401 Unauthorized: When the provided credentials are invalid. This tells the user they need to log in again.
403 Forbidden: When the user doesn't have permission to access a resource even after authentication.
404 Not Found: When the requested resource (e.g., a login page) is not found.
HTML Error Messages: Along with the HTTP status code, the server should provide a clear HTML error message on the web page. For example, if the username or password is incorrect, a message like "Incorrect username or password" can be displayed on the login page.

Why Error Messaging Matters:

User-Friendly: Error messages make the system more user-friendly by explaining issues in a way anyone can understand.
Problem Solving: Users can quickly identify what went wrong and take the necessary steps to fix it, like entering the correct password.
Security: Clear error messages help prevent brute force attacks, as attackers won't know if they're getting closer to the correct credentials.
Compliance: Some regulations and security standards require informative error messages to protect user data and privacy.

Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.


Had some help with chat GPT