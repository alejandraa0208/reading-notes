# Class 34 Notes

## Reading

### Review API Server Build

Explain the different between a query string parameter and a path parameter.

Query String Parameter: These are optional key-value pairs appended to the end of a URL after a question mark (?). They are used to filter or sort data, or for other purposes like search. For example, in http://example.com/items?color=blue, color=blue is a query string parameter that might tell the server to return only items that are blue.

Path Parameter: These are part of the URL's path and are used to identify a specific resource or resources. They are essential to the URL's structure. For example, in http://example.com/items/123, 123 is a path parameter that specifies a specific item (with ID 123) to be accessed or manipulated.

What would our API URL with a path id parameter be given the following information:

- Domain: http://our-site.com

- v3: 

- model name: stuff

- id: things

It would be: http://our-site.com/v3/stuff/things

We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

Imagine an API as a restaurant with a digital menu board (the "interface"). When you go to this restaurant, you can order various dishes. The digital menu (API interface) shows you what's available and how to order it (like GET for viewing, POST for creating new items, etc.). When you make a choice, the kitchen (server) prepares your dish and serves it to you. Similarly, when you make a request to the API (like asking for specific 'stuff'), the server processes it and sends back the information (like your order).

### Review Auth Server Build

Describe how you would use middleware to implement basic and bearer auth.

Basic Authentication: Middleware for basic auth typically involves extracting the Authorization header, which contains a Base64-encoded string of the username and password. The middleware decodes this string, verifies the credentials against a database, and either allows the request to proceed or denies it.

Bearer Authentication: With bearer token authentication, the middleware checks the Authorization header for a token (usually a JWT). It then validates this token (checking its integrity and expiration), and if valid, extracts the user information from it, allowing the request to proceed.

Describe the handshake necessary to implement OAuth.

Authorization Request: The client redirects the user to the authorization server with an authorization request.

User Consent: The user consents to the application's request for access.

Authorization Grant: The authorization server redirects back to the application with an authorization code.

Token Exchange: The application requests an access token from the authorization server by presenting the authorization code and its credentials.

Access Token Issued: The authorization server authenticates the application, validates the authorization code, and issues an access token (and optionally a refresh token).

Describe how Role Based Access Control works to a non-technical friend.

Imagine a theater play where everyone has a specific role: actors, directors, stagehands, etc. Each role has clear permissions about what they can do. For example, only the director can decide the play's scenes, actors perform, and stagehands manage the equipment.

In computer systems, RBAC works similarly. Users are given roles (like 'admin', 'editor', 'viewer'), and each role has specific permissions. An 'admin' might create and delete data, an 'editor' could modify it, and a 'viewer' might only be able to see it. This way, everyone only accesses what they need to, keeping the system secure and organized, just like our theater production.