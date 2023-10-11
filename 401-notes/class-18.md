# Class 18 Notes

## Reading

### AWS API Gateway Overview

What is Amazon API Gateway?

- Is a fully managed service from AWS that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.

Why is Amazon API Gateway an important part of the Serverless ecosystem?

- It's an important part of the Serverless ecosystem because it allows serverless applications to expose APIs to the outside world, enabling them to receive and respond to requests from clients like web browsers or mobile apps.

How does API Gateway integrate with other AWS services?

- API Gateway integrates with various AWS services, such as AWS Lambda, AWS Cognito for user authentication, and AWS S3 for serving static assets like images. It also supports custom integrations with your own back-end services.

### AWS API Gateway

What are the some benefits of using Amazon API Gateway?

- Benefits include easy API creation, auto-scaling to handle traffic, security through authentication and authorization, monitoring and logging, and the ability to create RESTful APIs or WebSocket APIs.

What two API types might you choose from?

- You can choose between REST APIs and WebSocket APIs. REST APIs are used for handling HTTP requests, while WebSocket APIs are for real-time communication over WebSocket connections.

### AWS DynamoDB Guide

What is DynamoDB?

- Is a fully managed NoSQL database service from AWS that provides fast and predictable performance with seamless scalability.

Under what circumstances would you recommend DynamoDB over MongoDB?

- DynamoDB might be recommended over MongoDB when you need a highly available, scalable, and fully managed NoSQL database without the operational overhead of managing servers and infrastructure.

### AWS DynamoDB

Explain to a non-technical friend how DynamoDB works.

- Amazon DynamoDB as a magical notebook that can store lots of information. It's like having a giant, super-fast, and super-reliable notebook in the cloud.

Now, in this notebook, you can write down all sorts of things, like to-do lists, your favorite recipes, or even customer orders if you're running a business. Each page in the notebook is like a table, and each line on a page is a record.

The cool thing is that you don't have to worry about where this notebook is or how it's kept safe. Amazon takes care of all that. It's stored on powerful computers that are always ready to handle your requests, no matter how many you throw at it.

So, when you want to add something new to your notebook, you just tell it what you want to write, and it's instantly recorded. If you want to find something, you can quickly search for it without flipping through pages, thanks to some clever indexing.

Plus, your notebook can grow with you. If you need more pages or more space, it magically expands. You don't need to worry about running out of room.

This notebook is super-fast, secure, and can handle lots of people reading from it or writing to it at the same time. It's like having the perfect notebook for your notes, lists, and data, all taken care of by Amazon's magical cloud technology.

### Dynamoose

What is Dynamoose?

- Is an ODM (Object Data Modeling) library for Amazon DynamoDB in JavaScript. It provides a way to work with DynamoDB in a more developer-friendly and model-driven approach.

What are some key features of Dynamoose?

- Key features of Dynamoose include type validation, built-in support for indexes, and the ability to define your data models using JavaScript classes. It simplifies DynamoDB interactions for developers.
