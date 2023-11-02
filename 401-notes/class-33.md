# Class 33 Notes

## Reading

### What is Role Based Access Control (RBAC)?

What is Role Based Access Control (RBAC)?

Role-Based Access Control (RBAC) is a method of regulating access to computer or network resources based on the roles of individual users within an enterprise. In this context, access is the ability of an individual user to perform a specific task, such as view, create, read, update, or delete (often termed as CRUD operations). With RBAC, access to resources is based on the role of the user, rather than the identity of the user.

Share some an example of RBAC including all possible CRUD operations and correlating roles.

Consider a content management system (CMS) for a company:

Admin: Can create, read, update, and delete (CRUD) all content, users, and roles.
Editor: Can read all content, create and update their content, but cannot delete any content.
Viewer: Can only read content.
Contributor: Can create content and read all content but cannot update or delete content.

What are the Benefits of RBAC?

Streamlined Management: Assigning roles to users simplifies permission management. When a new user is added to a system, administrators assign a role rather than individual permissions.
Improved Security: By adhering to the principle of least privilege (users only have the permissions they need to do their job), the risk of accidental misuse or malicious insider activity is reduced.
Scalability: As organizations grow and evolve, new roles can be easily created, and permissions can be updated across all users with that role.
Audit and Compliance: With clearly defined roles and responsibilities, it's easier to audit user activities and ensure regulatory compliance.

Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

react-cookie library

react-cookies component

Describe some react-cookie features.

Describe some react-cookies features.

react-cookie:

react-cookie is a popular library for handling cookies within React applications.
Provides hooks like useCookies for easy integration within functional components.
Allows server-side rendering of cookies, useful for universal or isomorphic applications.
Supports cookie encryption for added security.
react-cookies:

react-cookies is another library for managing cookies in React.
Uses React's context API to provide and manage cookie values.
Less popular and not as actively maintained as react-cookie.
Provides a simpler API but might lack advanced features compared to react-cookie.

Which library would you prefer would you prefer? Why?

I would prefer the react-cookie library over react-cookies for several reasons:

Popularity and Maintenance: react-cookie is more popular and appears to be more actively maintained. This typically means more frequent updates, better support, and a larger community for troubleshooting and sharing best practices.
Server-Side Rendering: The ability of react-cookie to handle server-side rendering can be crucial for certain applications that need this functionality.
Feature Set: With features like cookie encryption and hooks integration, react-cookie provides a more comprehensive toolset for modern React applications.