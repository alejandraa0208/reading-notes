# Class 03 Notes

## Review: ES6 Classes

1. Classes are a template for creating objects.

2.Can a class declaration be hoisted?

- No it cannot because they are not accessible before they are declared in the code.

3.How would you describe a constructor and contextual “this” to a non-technical friend?

- A constructor is like a recipe that instructs you how to create an object. "This" is like a magic word that refers to the object being created.

## Using Express Routing

1. Within Express, what does routing refer to?

- Routing refers to the process of determining how an application responds to a client request.

2.What is the difference between a route path and a route method?

- A route path specifies the URL patter or path the client is requesting. The route method defines the HTTP (CRUD).

3.When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

- It appropiate to add 'next' as a parameter to a route handler when you want to pass control to the next middleware function in the request-response cycle.

## Express Routing

1. What is an Express Router?

- Its like a mini express application that can be used to handle routes and middleware separately from the main express app.

2.By what mean do we initialize express.Router() in an express server?

- By creating an instance of the router and then defininf routes and middleware on the router object.

3.What do we use route middleware for?

- To perform actions on a specific route or a group of routes.

## Reflection

What are your learning goals after reading and reviewing the class README?

- My learning goals involve getting familiar with SQL database and when to use an express router.
