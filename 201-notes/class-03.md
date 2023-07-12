# Class 03 Notes

This page goes a little more in depth into HTML, CSS and Javascript.

## Learn HTML

1. When should you use an **unordered list** in your HTML document?

- You should use unordered list when you want to represent a collection of items that do not have a specific order.

2.How do you change the **bullet style** of unordered list items?

- You can use attributes or CSS.

3.When should you use an **ordered list** vs an **unorder list** in your HTML document?

- Depends on the type of list you are making. An ordered list should be used for things like steps or instructions.

4.Describe two ways you can change the numbers on **list items** provided by an **ordered list**?

- Using the attribute or CSS to change the numbers.

## Learn CSS

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

- Margin and Padding were the best duo you have ever seen. The way you can describe them individually makes sense why they are such a good pair.  Margin is like the protective shield, that could keep all the elements safe from surroundings. Margins greatest strength was being able to give elements enough breathing room and could prevent them from getting too close to other characters of the page. While Padding came off as warm and comforting. Such a nuturing presense that provided cushion between content and element borders. Together, they were able to help elements find their rightful place within the webpage bringing balance and structure to the user experience.

2.List and describe the four parts of an HTML elements box as referred to by the box model.

- The four elements are:
Content - which is the actual content of the webpage
Padding - space between content and element borders
Border - line or outline that surrounds the padding and content
Margin - space between element borders and any neighboring elements

## Learn JS

1. What data types can you store inside of an Array?

- Numbers, strings, booleans, arrays, and null

2.Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

- Yes the people array is valid and you can access the values you would use the array indexes

3.List five shorthand operators for assignment in javascript and describe what they do.

- += adds the right operand to the left and assigns the result to the left operand.
-= does the opposite of the += and subtracts.
*= multiplies the left operand by the right and assigns the result to the left.
/= divides the left operand by righ and assigns the result to the left.
%= calculates the remainder of the devision of the left operand by the right and assigns the result to the left.

4.Read the code below and evaluate the last expression and explain what the result would be and why.

 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

- the expression comes out to be (10 + false) + 'dog' which equals to '10falsedog'

5.Describe a real world example of when a conditional statement should be used in a JavaScript program.

- Form validation is a good use for conditional statements. Itll need the requirement that all fields are filled, validate email address anf verify passwords match.

6.Give an example of when a Loop is useful in JavaScript.

- Loop is useful when you want to repeat instructions or specific data to the usser.

### Things I want to know more about

Learning more short hand in JS so i do not have a messy code.

### LECTURE NOTES

JS Conditional Operatoors/ Truthy Falsy Values

Operators:

== weak equality - less strict, compares and matches

===  strong equality - more strict, checks to make sure data types are the same

Example:

'33' == 33 => true

'33' === 33 => false

&& logical And - true && false => false

| | logical Or - true | | false => true

Asking users to create an account with username and password but wont create it without the information needed.

! - logical inverse (not)

### CSS Box Model

Box model is every HTML element rendered in the browser has a box. The box has 4 layers. The layers are: size of content, padding - space around content, border - by default elements dont have a border unless you add it between padding and margin, and margin -the outer most layer, space between the border and any sibliing HTML element.  

HTML Composition -

CSS Properties -
