# Class 04 Notes

## React Docs - Forms

What is a ‘Controlled Component’?

- It is a concept in React,essentially a Javascript Library.

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

- It is bette to update the state as soon as they enter them because it provides a more responsive and interactive user experience.

How do we target what the user is entering if we have an event handler on an input field?

- You need to access the event object thats passed to the event handler function since it contains informaiton about event and the target element.

## The Conditional (Ternary) Operator Explained

Why would we use a ternary operator?

- It is used to write conditional statements. It is three operands: a condition, a value to return if condition is true and value to return if the condition is false.

Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

new statement:

console.log(x === y);
