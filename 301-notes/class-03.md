# Class 03 Notes

## React Docs - lists and keys

What does .map() return?

- It returns a new array with the results of calling a provided function on every element in the calling array.

If I want to loop through an array and display each value in JSX, how do I do that in React?

- Use .map() to iterate over the array and return JSC elements for items.

Each list item needs a unique key.

What is the purpose of a key?

- To help React identify which items have changed, added or removed.

## The Spread Operator

What is the spread operator?

- It is used to expand or unpack elements from arrays, objects or other values.

List 4 things that the spread operator can do.

- Combine arrays, clone arrays and objects, pass elements of an array as function arguments and create new objects with modified properties.

Give an example of using the spread operator to combine two arrays.

- const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const combinedArray = [...array1, ...array2];
console.log(combinedArray);

Give an example of using the spread operator to add a new item to an array.

- const originalArray = [1, 2, 3];
const newArray = [...originalArray, 4];
console.log(newArray);

Give an example of using the spread operator to combine two objects into one.

- const obj1 = { x: 1, y: 2 };
const obj2 = { z: 3 };
const combinedObject = { ...obj1, ...obj2 };
console.log(combinedObject);

## Things I Want To Know More About

n/a
