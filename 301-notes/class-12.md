# Class 12 Notes

## Status Codes Based on REST Methods

In your own words, describe what each group of status code represents:

100’s = indicate provisional responses

200’s = indicates that the request ws recieved and processed successfully by the server

300’s = indicate that further action needs to be taken by the client to fulfill the request

400’s = indicates that there was an issue with the clients request

500’s = indicates that there was an issue on the servers end while processing request

What is a status code 202?

- indicates that the request has been accepted for processing but the processing may not be completed yet.

What is a status code 308?

- indicated that the requested resource has been permanently moved to a different location.

What code would you use if an update didn’t return data to a client?

- You could use a status code 204.

What code would you use if a resource used to exist but no longer does?

- Status code 410

What is the ‘Forbidden’ status code?

- 403 and it indicated that the server understood the request but the server refuses to authorize it.

## Build a REST API with Node.js, Express & MongoDB

Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- Storing sensitive information like database connection strings, API keys and other configuration values in environment variables rather than hardcoding.

What is middleware?

- Is a software component that acts as an intermediary between two systems or components.

What does app.use(express.json()) do?

- It is middleware that parses incoming JSON data from requests and makes it accessible in the 'req.body' object.

What does the /:id mean in a route?

- It captures a dynamic value from the URL.

What is the difference between PUT and PATCH?

- PUT is the method is used to update or replace the entire resource identified by the given URL.

PATCH is the method to make partial updated to a resource.

How do you make a default value in a schema?

- When you define the schema for database models you can specify default values for certain fields.

What does a 500 error status code mean?

- It is a generic error message returned by the server when an unexpected condition was encountered that prevented it from fulfilling the request.

What is the difference between a status 200 and a status 201?

- Status 200: Indicates that the request has succeeded. used for successful responses to GET, PUT, PATCH and DELETE request.

Status 201: Indicated successful creation of a resource. Returned in response to POST requests.
