# Class 15 Notes

## What is OAuth?

What is OAuth?

- It is an open standard protocol that allows third-party applications to access the users data on a service without showing credentials.

Give an example of what using OAuth would look like.

- Say you want to log into a website using your google account, it uses an OAuth to request basic infor from google without showing your credentials.

How does OAuth work? What are the steps that it takes to authenticate the user?

- 1: User Requests Authorization

2: Redirect to Authorization Server

3: User Grant Authorization

4: Exchange Authorization Code for Token

5: Access Resouces

6: Access Token Expiry and Refresh

What is OpenID?

- It is an authentication protocol that allows users to log into multiple websites using a single digital identity.

## Authorization and Authentication flows

What is the difference between authorization and authentication?

- Authorization process of verifying the identity of a user, system or entity.

Authentication is the process that determines what actions or resources a user, system or entity allowed to access or perform.

What is Authorization Code Flow?

-

1: Client refirects the user to the authorization servers login page.

2: User logs in and apporves the requested permissions

3: Authorization server provides the client with an authorization code.

4: Client exchanges the authorization code for an access token from the server.

5: Client can then use the access token to access the user's resources.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

- PKCE is an extension to the Authorization Code Flow that adds an extra layer of security to public clients (e.g., mobile apps, single-page apps). It prevents attackers from stealing the authorization code and exchanging it for an access token. PKCE involves generating a code verifier and a code challenge that the client uses to obtain an access token.

What is Implicit Flow with Form Post?

- The Implicit Flow with Form Post is an OAuth 2.0 flow suitable for clients that are implemented entirely in the browser (such as single-page apps). In this flow, the access token is returned directly in the URL fragment after the user logs in, and the client uses JavaScript to extract it and hide it from the URL.

What is Client Credentials Flow?

- The Client Credentials Flow is used by clients (applications) to authenticate themselves directly with the authorization server. This is typically used for machine-to-machine communication, where the client itself (not a user) needs access to resources.

What is Device Authorization Flow?

- The Device Authorization Flow (Device Code Flow) is designed for devices with limited input capabilities (such as smart TVs or gaming consoles). The user interacts with a secondary device (e.g., a smartphone) to authorize the primary device to access resources on their behalf.

What is Resource Owner Password Flow?

- The Resource Owner Password Flow allows clients to request an access token using the user's username and password. This flow is less secure and is generally discouraged, but it might be used when the client is highly trusted and there are no better options available.

These flows provide different ways to obtain access tokens in OAuth 2.0 based on the specific requirements and capabilities of the client application and the security considerations involved.
