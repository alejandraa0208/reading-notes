# Class 29 Notes

## Reading

### Extracting State Logic into a Reducer

What is the motivation for adding a reducer?

- Reducers are motivated by the need for more predictable and maintainable state management, especially in complex state logic that involves multiple sub-values or when the next state depends on the previous one.

What are actions in the context of a reducer? How are they different than setting state directly?

- In the context of a reducer, actions are objects that represent a description of the "action" to be taken. They typically contain a type property to describe the kind of state transition, and they might also carry some data (often referred to as payload).

Setting state directly (e.g., using setState in class components or useState in functional components) updates the state based on the new value you provide. Actions, on the other hand, just describe the update that should happen. The reducer then interprets that description and decides how the state should change in response.

What common list operation is useReduce named for, and why?

- The name useReducer is a play on the reduce function commonly found in many programming languages, including JavaScript. The reduce function takes a list (or array) and reduces it down to a single value by successively applying a function. In the context of useReducer, you're effectively "reducing" a series of actions into a new state based on the previous state.

When should you switch from useState to useReducer?

- Complex State Logic: When the logic to update the state becomes intricate or involves multiple sub-values.

Interdependent State: If the next state depends on the previous state. While this can be handled with useState using functional updates, useReducer can provide clearer semantics in such scenarios.