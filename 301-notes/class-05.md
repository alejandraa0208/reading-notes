# Class 05 Notes

## React Docs - Thinking in React

What is the single responsibility principle and how does it apply to components?

- It is a principle in software design that states that a component or module should have only one reason to change. When applied to a component it means it should ideally have a single responsibility/purpose.

What does it mean to build a ‘static’ version of your application?

- It involves creating the UI without any interactivity or dnamic behavior.

Once you have a static application, what do you need to add?

- You need to add state management and event handling, components to respond to user interactions.

What are the three questions you can ask to determine if something is state?

- Does it change over time?

Can it be computed from other state or props?

Does it affect the components rendering?

How can you identify where state needs to live?

- Identify every component that renders something based on that state.

State should live in the common parent component if shared by multiple child components.

## Higher-Order Functions

What is a “higher-order function”?

- It is a function that operate on other functions, either by taking them as arguments or by returning them.

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

- The second line is defining and returning an inner function that takes a parameter 'm' and checks whether 'm' is greater than the value of 'n', which is the parameter passed to the outer function.

Explain how either map or reduce operates, with regards to higher-order functions.

- Map is used to transform each element of an array by applying a provided callback function to each element and creating a new array with the results of those transformations.
