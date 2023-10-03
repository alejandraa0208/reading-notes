# Class 11 Notes

## Reading

### Event Driven Programming

What native Node.js module allows us to get started with Event Driven Programming?

- The 'events' module allows to get started with Event Driven Programming. Provinging a foundation for working with events and event-driven programming.

What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

- Lies in the organization and encapsulation of code.

Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

Imagine you're running a restaurant, and you have a team of chefs, waitstaff, and customers. Each person in the restaurant is like a small program that can do certain things. Now, instead of shouting orders or instructions to each other, everyone uses a bell system.

Customer Bell: Customers ring a bell when they're ready to order food.
Chef Bells: Chefs have bells that ring when an order is ready to be served.
Waitstaff Bells: Waitstaff have bells that ring when they're needed to serve a dish.
Here's how this relates to Node.js on the backend:

In Node.js, we have different parts of our program (like chefs, waitstaff, and customers) represented by different pieces of code.
These code parts can communicate by sending and receiving "bells," which are like events.
When a customer wants to order (sends an event), the kitchen (your Node.js server) knows to start preparing the order.
When the order is ready (another event), the waitstaff (another part of your code) knows to serve it to the customer.
