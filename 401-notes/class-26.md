# Class 26 Notes

## Reading

### React Quick Start

What are the building blocks of a React app?

- Components, props, state, hooks, and context.

What is the difference between an HTML element and a React component?

- HTML is a standard piece of the web markup language that represented by tags and react component is a custom element thtat encapsulates code for rendering UI and handling logic.

What is JSX and why do we use it?

- Is a syntax extension for Javascript and we us it because it makes UI code more readable and expressive.

Describe the process of embedding JavaScript expressions in JSX.

- you embed the JS expression in JSX by wrapping them in curly braces.

Does React or JSX have any special features for iteration or conditional logic?

- You can use Javascripts map function to iterate over items and you can use ternary operators or short-circuit evaluation for conditional logic.

How does React know to respond to a user’s inputs?

- React uses a synthetic event system. When a user interacts with a React component (e.g., clicking a button), React creates synthetic events that simulate the corresponding native browser events. Event handlers (e.g., onClick, onChange) can be added to components to respond to these events.

What word indicates that a React component manages data with a Hook?

- The word use in front of function names, like useState, useEffect, signifies that a component is using a hook.

How can two react components share data?

- Parent-child: through props, sibling-sibling: lift the state up to their closest common ancestor and then pass down through props, and using context or state management libraries.

### Render and Commit

What are the three steps of refreshing a React UI?

- Render, reconciliation and commit

How do you trigger updates to a component after the initial render?

- Changing the state or props of a component will trigger a re-render.

Does React recreate DOM nodes on every rerender?

- No, React uses the Virtual DOM to determine what changes are needed and then updates only the necessary parts of the actual DOM, making it more efficient.

After React has updated the DOM, what still needs to happen before the user sees the change?

- Browsers perform a process called painting. This is when the changes in the DOM are drawn or rendered on the screen. This step happens after the DOM has been updated but before the user sees the changes.
