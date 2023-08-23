# Class 08 Notes

## API Design Best Practices

What does REST stand for?

- Stands for Representational State Transfer

REST APIs are designed around a set of architectural principles and constraints.

What is an identifier of a resource? Give an example.

- It can be a URI and an example can be <https://api.example.com/products/123>

What are the most common HTTP verbs?

- GET, POST, PUT and DELETE

What should the URIs be based on?

- Based on the resources that the API exposes.

Give an example of a good URI.

- <https://api.example.com/customers/789/orders/12345>

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- It means the API needs a large number of small request to retrieve or manipulate data. Its considered a bad thing because it can increase network overheade and slow performance.

What status code does a successful GET request return?

- It returns 200 OK

What status code does an unsuccessful GET request return?

- The code could be:

404 Not Found

or

400 Bad Request

What status code does a successful POST request return?

- It returns a 201 Created

What status code does a successful DELETE request return?

- It returns 204 No Content
