# Class 09 Notes

## Functional Programming Concepts

What is functional programming?

- It is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutbale data.

What is a pure function and how do we know if something is a pure function?

- Its a fundamental concept in functional programming. It produces the same output for the same input and doesnt have any observable side effects and replace a function call with its outputs without affecting program behavior.

What are the benefits of a pure function?

- Some benefits are predictability, testability, caching and memoization.

What is immutability?

- It is a concept where once data is created, it cannot be changed.

What is Referential transparency?

- It is a property of expressions in a program.

## Node JS Tutorial for Beginners #6 - Modules and require()

What is a module?

- Refers to a self-contained unit of code that has a specific functionality. Used to organize code into manageable and reusable components.

What does the word ‘require’ do?

- Used in environments like Node.js to import modules.

How do we bring another module into the file the we are working in?

- Ensure the module you want to use is properly defined and exported in its own file. Then, in whatever file you want to use that module 'require' imports it.

What do we have to do to make a module available?

- Create a JS file, define functions, objects or variables to export, and then use 'exports' to specify what should be accessible outside of the module.
