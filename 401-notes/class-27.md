# Class 27 Notes

## Reading

### Thinking in React

Summarize the five steps of thinking in react.

- Break the UI into a component hierarchy: Look at the design/mockup and break it down into components. A general rule is if a part of your UI is used several times or is complex enough on its own, it should be a standalone component.

- Build a static version in React: Create a version that takes your data model and renders the UI but has no interactivity. This step doesn't involve state.

- Identify the minimal (but complete) representation of UI state: Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand.

- Identify where your state should live: Determine which component should own the state. Generally, it should live in the highest common ancestor of components that need it.

- Add inverse data flow: If one component changes another component’s state, pass callbacks to the component that will be responsible for handling the state modifications.

### State: A Component’s Memory

What is one reason a local variable isn’t sufficient for managing a React component?

- Local variables don't trigger re-renders. React's reactivity is based on its state management. When state changes, React knows it needs to re-render the affected components. A local variable doesn't have this capability, meaning changes to it won't cause the component to update.

What is the argument to the useState hook, and what are the two parts of its return array?

- Argument: The initial state value.

Returning array: The current state value and a function to update that state value.

How can Component A access state from Component B?

Directly: Components cannot directly access the state of their siblings or children. They can only receive state through props.

Through Parent: If two components need to share state, a common pattern is to lift the state up to their nearest common ancestor. This ancestor component manages the state and passes it down to both Component A and Component B via props.

Using Context: React’s Context API allows components to share values without having to pass props through every level of the tree.

State Management Libraries: Libraries like Redux, MobX, or Zustand provide more global state management solutions where any component can access or update the state without prop drilling.
