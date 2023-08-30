# Class 13 Notes

## CRUD Basics

Which HTTP method would you use to update a record through an API?

- You would use "PUT" or "PATCH".

PUT is used to update or replace the entire resource at the specific URL with the new representation provided in the request.

PATCH is used to make partial updates to a resource.

Which REST methods require an ID parameter?

- The REST methods that require an ID parameter are GET, PUT, PATCH and DELETE.

## Speed Coding: Building a CRUD API

What’s the relationship between REST and CRUD?

- REST often maps to CRUD to manage resources over the web. REST provides a set of principles for designing networked applications and CRUD represents the basic operations that can be performed on those resources.

If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

- Step 1: Identify Resources: Determine data entities you want to expose and manage through APIs and they become a resouce.

Step 2: Define Endpoints: Create a set of endpoints for each resource.

Step 3: Implement Data Storage: Choose a data storage and manage the resource data.

Step 4: Implement Controller Logic: Create controller functions for each endpoint that handle the logic associated with the corresponding CRUD operation.

Step 5: Handle Response and Errors: Return appropiate HTTP status codes and response bodies based on outcome of each request.
