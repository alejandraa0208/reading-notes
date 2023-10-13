# Class 19 Notes

## Reading

### AWS SQS vs SNS

What is the difference betweeen SQS and SNS?

- SQS is a message queue service used for decoupiling the compoenets of a cloud application and they can work together independently. SNS is a publish-subscribe service for sending notification and messages to a distributed set of recipients or endpoints.

What are some use cases for both SNS and SQS?

- Some use cases are SQS manages tasks asychronously, load leveling and decoupling services. SNS is used for broadcasting messages to multiple subcribers like push notifications and event triggers.

### AWS SNS and SQS

Describe how to use SQS and SNS in a “fanout” pattern.

-SNS can be used to broadcast messages to mulitple SQS queues. Each queue processes the message as needed.

Explain how “push notifications” work, using SNS.

- SNS enables them by allowing you to send messages to a variety of endpoints like mobile devices, email or Lambda functions.

### SQS and SNS Basics

How might a large scale, distributed application make use of a Queue system like SQS?

- In a large-scale, distributed application, SQS can be used to manage the flow of tasks and ensure that they are processed efficiently across multiple components or services. It helps prevent overloading one part of the system.
