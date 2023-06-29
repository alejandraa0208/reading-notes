# Class 08 Notes 

Looping code - any code that runs more than once. 

For Loop - 
syntax = for (incrementor - break condition - updater) {
    all the code to be repeated;
}
ex - 
for (let i = 0; i<10; i++) {}
While Loop - syntax = while 
 ## Example of looping code 


for (let i = 0; i < 10; i++) {
    console.log('i is equal to :', i);
    debugger;
}

function askName() {
    let name = prompt('What is your name?');
    while(!name) {
        name = prompt('No I really need your name');
    }
    alert('Welcome ' + name)
}


for (let i = 0; i < Number; i--) {
    document.write('<img src = ')
}

Math.random();  = returns a random number between 0 and 1. 

## Reflection and Discussion 

1. What is an expression in JavaScript?

- An expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate. 

2. Why would we use a loop in our code?

-  It's a quick and easy way to do something repeatedly.

3. When does a for loop stop executing?

- The for loop stop executing once a specified condition evaluates to falst. 

4. How many times will a while loop execute?

- A while loop will execute as long as a specific condition evaluates to true. 