# Class 07 Notes

## Reading

### Intro to JWT

What is a JSON Web Token (JWT)?

- Its a compact, self-contained means of representing and transmitting information between partied as a JSON object. Used for securely transmitting formation between client and a server.

When should we use JSON Web Tokens?

- Are used for authentication, authorization and single sing-on.

Claims are expected in which structural component of a JWT?

- They are expected in the payload of a JWT.

### Are JWTs Secure?

If I get a JWT and I can decode the payload, how can we call that secure?

- By using a digital signature like a secret key.

If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

- Sender and reciever must both know the secret key.

Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

- Think of it as sending a secret message to someone. Sender also sends a key with the message that only the reciever can see. Once they recieve the message with the key the reciever can use the key to validate any messages.

## Videos

### JWTs Explained

Why use JWT?

- It is used to secure information for outside parties.

JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

- JWT is a tiny, smart package. It's like putting the key and the information in a small, sealed envelope. This envelope not only contains the key (like a username or ID) but also a little note that says, "I trust you because I signed this."

Now, think about sending this envelope through the internet. It's so small and has everything your friend needs. Your friend can open it, read the note, and use the key to access the information, all without needing to ask you for more details. It's like magic!

So, JWT is like a digital envelope that's super small, easy to send, and carries everything needed to verify trust and access information. It's a nifty way to make sure the right people can get the right stuff online.

What are the three components (the structure) of a JWT signature?

- Header, Payload and signature

## Reflection

I want to get more clairty for setting and creating APIs and servers by scratch.
