# Class 36 Notes

## Reading

### Dan Abramov Redux Tutorials

What is the first principle of Redux?

- The first principle of Redux is that all application state is held in a single, immutable state object within a single store. This makes the state of your entire application predictable and easier to track. Any change in the application's state results in a new object being created to represent that state, which helps prevent unintended side-effects.

what is a store and what do we use our reducers for within that store?

- In Redux, a store is an object that brings together the state, actions, and reducers that make up your application. It can be thought of as a container that holds the state of the application.

Reducers are pure functions that take the current state of the application and an action as arguments and return a new state. The reducer functions are responsible for handling state transitions that result from actions. Reducers are used within the store to manage the complexities of state transitions and to ensure that state changes are predictable and transparent.

Name three Redux store methods given to us by createStore and describe their use.

- The createStore function in Redux provides you with a store that has several methods, three of which are:

getState(): This method retrieves the current state of the Redux store. It is useful whenever you need to get the current value of your application state.

dispatch(action): This method is used to dispatch an action to the store. An action is a plain JavaScript object that represents an intention to change the state. Dispatching an action is the only way to trigger a state change.

subscribe(listener): This method allows you to listen for changes to the store's state. It accepts a callback function that will be executed every time an action is dispatched to the store, after the reducers have updated the state.

Explain to a non-technical recruiter what combineReducers() does and why it is useful.

- Imagine you have a complex project to manage with different teams working on different parts. To make it manageable, you divide the project into sections and assign each section to a specialized team. Each team manages its part independently but needs to make sure their section aligns with the overall project plan.

In Redux, combineReducers() is like the project manager. It takes all the different parts of the application's state, which are managed by different "teams" (reducers), and combines them into one cohesive "project plan" (state object). This way, each team (reducer) can work independently on their part of the state, and combineReducers() ensures they all fit together in a way that makes sense for the whole application.

This is useful because it helps keep the application organized, makes it easier to maintain, and allows you to scale your application by adding new features without getting overwhelmed.
