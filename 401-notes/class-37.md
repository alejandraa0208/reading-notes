# Class 37 Notes

## Reading

### Multiple Reducers Example

Why create multiple reducers?

- In Redux, it's common to create multiple reducers when the application grows complex. Each reducer is responsible for managing a specific slice of the application's state. This modular approach helps keep the code for managing different data domains separate and easier to maintain. It also makes it easier to understand which reducer is responsible for which part of the state and to reuse reducers across different parts of the application.

How would you combine multiple reducers?

- To combine multiple reducers, Redux provides a utility function called combineReducers. This function takes an object as an argument, with the shape of the state object managed by each reducer

How will you manage state as an immutable object? why?

- In Redux, the state should be treated as immutable because immutability ensures that the state is not changed in an unpredictable way, which can lead to bugs that are hard to track down. To manage state immutably, you should never modify the state object directly. Instead, you should return a new object that represents the updated state.

### Redux Docs: Using Combined Reducers

combineReducers is a utility function to simplify the most common use case when writing reducing functions.

Explain how combineReducers assembles the new state tree.

- combineReducers assembles the new state tree by calling each child reducer with its slice of the state and the current action. Each child reducer is responsible for updating its piece of the state, and combineReducers then combines those results into a single state object. The structure of the state object matches the keys of the passed reducers.

How would you define initial state in an app using combineReducers?

- When using combineReducers, you typically define the initial state within each individual reducer. Each reducer provides its initial state as the default parameter value:

function usersReducer(state = initialUsersState, action) {

  // reducer logic

}

function postsReducer(state = initialPostsState, action) {

  // reducer logic

}

const rootReducer = combineReducers({

  users: usersReducer,

  posts: postsReducer

});

initialUsersState and initialPostsState are defined within their respective reducers. The combined initial state is then the result of combining these individual initial states.

### Redux Docs: Combined Reducer Syntax

Why will you want to split your reducing functions as your app becomes more complex?

- As applications grow more complex, it becomes increasingly difficult to manage the entire state in a single reducer function. Splitting reducers into smaller functions that handle specific slices of state keeps the logic manageable and organized. It's easier to debug, test, and maintain several smaller, more focused reducers than one monolithic reducer function.

The combineReducershelper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

What is a popular convention when naming reducers?

- A popular convention when naming reducers is to name them after the slice of state they manage. For example, a reducer that manages a list of users might be called usersReducer. This makes it clear what part of the state tree each reducer is responsible for.
