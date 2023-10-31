# Class 31 Notes

## Reading

### Choosing the State Structure

Summarize the five principles for structuring state.

**Minimal State**: Only store the minimal amount of state your UI needs to function. Calculate other required values on-demand from this minimal state.

**Lifting State Up**: When multiple components need to access and modify the same piece of state, move that state to their closest common ancestor.

**State vs Props**: Be clear about which values should be stateful and which ones should be passed down as props. If a value is passed in from a parent and doesn't change in the component, it should be a prop.

**Immutable State**: When updating state, always create a new state object rather than mutating the existing one. This makes state changes predictable and is necessary for components to correctly detect changes for rendering.

**Splitting State Logic**: Divide state logic into smaller pieces rather than a monolithic state object, especially for larger applications. This can make the application more manageable and optimized.

### Passing State Deeply with Context

What problem do Contexts aim to solve?

Context aims to solve the problem of "prop drilling" in React applications. Prop drilling refers to the process of passing data from a top-level component down multiple levels through intermediate components that might not even need that data. It can make components less reusable and harder to refactor. Context allows for easier sharing of values like themes, locale preferences, or authenticated user information to any component, without having to explicitly pass them via props at every level.

What is one technique to try before useContext?

Before jumping to useContext, one should consider "lifting the state up". This involves moving the state to a closer common ancestor of the components that need it. It can make the data flow more explicit and easier to follow without introducing the complexity of context.

What hook complements useContext for complex applications?

For complex applications, the useReducer hook often complements useContext. useReducer allows for more organized state management by maintaining state logic in a reducer function. When used together, useContext can provide access to state (and dispatch functions) globally across components, and useReducer can handle complex state logic in a predictable manner.
