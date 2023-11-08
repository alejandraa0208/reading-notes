# Class 38 Notes

## Reading

### async actions

Why use Redux middleware?

- Redux middleware is used to extend Redux with additional functionality. It provides a third-party extension point between dispatching an action and the moment it reaches the reducer. Middleware can be used for logging, crash reporting, performing asynchronous tasks, etc. In the context of asynchronous actions, middleware like Redux Thunk or Redux Saga can handle side effects such as data fetching or accessing browser APIs, which are tasks that don’t fit into Redux’s basic action-reducer flow.

Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

- In the Redux async data flow:

An action creator dispatches an asynchronous action. This is often done through a function that returns a function (thunk) that takes dispatch and getState as arguments.
Middleware intercepts this action. If it's a function (thunk), middleware executes it, allowing for asynchronous operations to run.
Inside the thunk, you may dispatch other actions to notify the application that an asynchronous operation has begun.
The async operation executes, and upon completion or failure, the thunk dispatches a new action reflecting the result (usually a success or error action).
This dispatched action is a regular object and flows through any other middleware and then to the reducers, which update the state accordingly.
The UI may then re-render based on the new state.

How are we accommodating async in our Redux app?

- We accommodate async in a Redux app by using middleware such as Redux Thunk or Redux Saga. These tools allow us to perform async logic, such as API calls, and dispatch actions asynchronously when the operation completes or fails. This helps in keeping the action creators and reducers clean and focused on their primary responsibilities.

### thunk middleware

Why would you need redux-thunk middleware?

- Redux-thunk middleware is needed when you want to perform asynchronous operations or side effects in your Redux action creators. Redux itself only supports synchronous data flow, and thunks provide a way to extend Redux to support asynchronous actions.

Redux Thunk middleware allows you to write action creators that return a function instead of an action.

Describe how any return value from the inner thunk function will be made available.

- Any return value from the inner thunk function can be used by the component dispatching the action. When the thunk is executed by the middleware, it can return a value, such as a promise. This return value can then be handled by the component to, for example, display loading states, handle the fulfilled promise (like a response from an API call), or catch errors from a rejected promise. This makes the return value of the thunk very flexible and can be integrated with the component's lifecycle methods or hooks for managing local state and UI updates.
