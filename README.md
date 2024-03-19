# Day 1
# Variables, Operators & Assignments
## Variables
<p>Variables are containers for storing data values. They are used to label and store information that can be referenced and manipulated in a program.</p>

<p>In JavaScript, variables are declared using the var, let, or const keywords.</p>

<ul><li><strong>var</strong> is the traditional way of declaring variables in JavaScript.</li>
<li><strong>let</strong> allows you to declare variables that can be reassigned.</li>
<li><strong>const</strong> declares variables with constant values, which cannot be reassigned.</li></ul>
<p>Naming Convention: Variable names can consist of letters, digits, underscores, and dollar signs. They must begin with a letter, underscore, or dollar sign. Variable names are case-sensitive.

Scope: Variables can have local or global scope. Variables declared inside a function are local to that function, while variables declared outside any function have global scope.

Hoisting: In JavaScript, variable declarations are hoisted to the top of their containing scope during compilation. However, only the declaration is hoisted, not the initialization.</p>


## Operators

### Arithmetic Operators 

<p>Arithmetic Operators are used to perform mathematical calculations.</p>

<p>Addition (+), Subtraction (-), Multiplication (*), Division (/), Modulus (%).</p>

  
### Assignment Operators

<p>Assignment Operators are used to assign values to variables.</p>

<p>Simple assignment (=), Addition assignment (+=), Subtraction assignment (-=), etc.</p>


### Comparison Operators

<p>Comparaison Operators are used to compare values.</p>

Equal to (==), Not equal to (!=), Greater than (>), Less than (<), etc.
Logical Operators: Used to combine and manipulate logical expressions.

Logical AND (&&), Logical OR (||), Logical NOT (!).

### Bitwise Operators 

<p>Bitwise Operators are used to perform bitwise operations on integers.</p>

Bitwise AND (&), Bitwise OR (|), Bitwise XOR (^), Bitwise NOT (~), etc.

<h4>Unary Operators</h4>: Operates on a single operand.

Increment (++), Decrement (--).

<h4>Ternary Operator</h4>: A conditional operator that evaluates a condition and returns one of two values based on whether the condition is true or false.

Syntax: condition ? value1 : value2


# Day 2
## Strings and Arrays
#### Strings

<p>A string is a collection of one or more characters, which may include letters, numbers, or symbols. Strings in JavaScript are primitive data types that are immutable, which means they do not change.
Strings are one of the most essential aspects of programming to comprehend since they are how we display and manipulate text, and language is our primary means of communicating and understanding through computers.</p>

<strong>Creating and seeing the output of strings</strong>
There are three methods to write a string in JavaScript: within single quotes (' '), double quotes (" "), or backticks. The quotation type must be the same on both sides, however all three types may be used throughout the script.

Strings with double and single quotations are practically the same. There is no tradition or formal preference for single- or double-quoted strings; all that counts is that they are consistent among project program files.

'This string contains single quotes.';

"This string uses double quotes." ;
this post.

This string includes backticks.';

The simplest method to see the output of a string is to publish it to the console using console.log().

console.log("This is a string in the console.");

Output
This is a string from the console.

Another easy approach to produce a value is to send an alert popup to the browser using alert():

alert("This is a string in an alert.");

Running the above code will result in the following output in the browser's user interface

#### Arrays

<p>An array is a special type of object used to store multiple values in a single variable. Arrays can hold various data types, including numbers, strings, objects, and even other arrays.</p>
<p>Arrays are declared using square brackets []. You can initialize an array with elements inside the brackets, separated by commas.

For example
  
var myArray = [1, 2, 3, 4, 5];</p>

<p>Accessing Elements: Individual elements within an array can be accessed using square brackets [] with the index of the element. Index start from zero [0].

For example:
var firstElement = myArray[0]; // Accessing the first element
var thirdElement = myArray[2]; // Accessing the third element</p>

<p>Array Length: The length property of an array returns the number of elements in the array.
  
For example

var arrayLength = myArray.length;</p>

<strong>Modifying Arrays: You can modify arrays by adding, removing, or updating elements.</strong>

##### Adding Elements: 
<p>We use the push() method to add elements to the end of an array.

myArray.push(6); // Adds 6 to the end of the array</p>

##### Removing Elements: 
<p>We use pop() to remove the last element, shift() to remove the first element, or splice() to remove elements at specific positions.</p>

##### Updating Elements 
When assigning a new value to a specific index to update the element.

myArray[0] = 10; // Updates the first element to 10

# Day 3
## Functons

<p>In JavaScript, functions are blocks of reusable code that perform a specific task or calculate a value. This avoids the need to write the same code again and over. It assists programmers in building modular code. Functions allow a programmer to break a large program into smaller, more manageable functions.
 JavaScript, like any other modern programming language, has all of the capabilities required to construct modular code with functions. You must have seen functions such as alert() and write() in previous chapters. We used these methods repeatedly, but they had only been defined in core JavaScript once. JavaScript also allows us to define custom functions.</p>

##### Function Declaration: 
<p>Functions in JavaScript can be declared using the function keyword followed by the function name, parameters (if any), and the function body enclosed in curly braces. For example:</p>

<p>function greet(name) {
    console.log("Hello, " + name + "!");
}</p>
<h5>Function Expresion: </h5>

<p>Functions can also be defined using function expressions, where a function is assigned to a variable. For example:</p>

<p>const greet = function(name) {
    console.log("Hello, " + name + "!");
};</p>

##### Anonymous Functions: 

<p>Functions without a name are called anonymous functions. They are often used as callback functions or immediately invoked function expressions (IIFE). For example:</p>

<p>setTimeout(function() {
    console.log("This is an anonymous function.");
}, 1000);</p>


##### Function Parameters: 
<p>Functions can accept zero or more parameters, which are placeholders for values that the function will work with. Parameters are listed within the parentheses of the function declaration. For example:</p>

<p>function add(a, b) {
    return a + b;
}</p>
<h5> Return Statement: </h5>

<p>Functions can return a value using the return statement. When a function encounters a return statement, it immediately exits and returns the specified value. For example:</p>

<p>function add(a, b) {
    return a + b;
}</p>

##### Function Invocation: 

<p>Functions are executed or called using their name followed by parentheses (). For example:</p>

<p>greet("John");</p>

<ul><li><strong>Scope</strong>: Functions introduce their own scope in JavaScript. Variables declared within a function are local to that function by default and cannot be accessed from outside the function unless explicitly returned or using closure.</li>

<li><strong>Hoisting</strong>: Function declarations are hoisted in JavaScript, meaning they are moved to the top of their containing scope during the compilation phase. This allows you to call a function before it is declared in your code.</li>

<li><strong>Nested Functions</strong>: JavaScript allows functions to be nested within other functions. These nested functions have access to the variables and parameters of their containing (outer) function, which can be useful for creating closures.</li>

<li><strong>Arguments Object</strong>: Functions in JavaScript have access to a special arguments object, which is an array-like object containing all the arguments passed to the function. This object can be used to access arguments dynamically, even if they are not explicitly defined in the function signature.</li></ul>

<i>Functions are fundamental building blocks in JavaScript, providing a way to organize and reuse code, encapsulate functionality, and create modular and maintainable codebases.</i>

# Day 4
## Booleans

### Understanding Boolean and Conditional Values:
##### Boolean values in JavaScript represent two values: true or false.

<p>They are used to control the flow of programs, determine conditions, and make decisions.
Boolean values are the result of comparison operations, logical operations, or can be explicitly set.</p>

##### Examples of boolean values: true, false.

##### Use Conditional Logic with If Statements:

<p>Conditional statements in JavaScript allow you to execute different code blocks based on specific conditions.
The if statement is the most basic form of conditional statement.</p>
Syntax:

<p>if (condition) {
    // code to execute if condition is true
};</p>

<p>The code block inside the if statement is executed only if the condition evaluates to true.
You can also use else statement to execute code when the condition is false.</p>

##### Comparison with the Equality Operator:

<p>The equality operator == compares two values and returns true if they are equal, false otherwise.
It performs type coercion, meaning it tries to convert both values to a common type before making the comparison.
Example:</p>

console.log(5 == 5); // true
console.log(5 == '5'); // true (type coercion)
console.log(5 == 6); // false


##### Comparison with the Strict Equality Operator:

<p>The strict equality operator === compares two values without performing type coercion.
It returns true if the values are of the same type and have the same value, false otherwise.
Example:</p>

console.log(5 === 5); // true
console.log(5 === '5'); // false (no type coercion)
console.log(5 === 6); // false


##### Practice comparing different values:

<p>It's important to practice comparing different values using both equality and strict equality operators to understand their behavior.
This helps in understanding how JavaScript handles type coercion and strict type checking.
</p>

##### Comparison with the Inequality Operator:

<p>The inequality operator != checks if two values are not equal and returns true if they are not equal, false otherwise.
It performs type coercion similar to the equality operator.
Example:</p>


console.log(5 != 5); // false
console.log(5 != '5'); // false (type coercion)
console.log(5 != 6); // true

##### Comparison with the Strict Inequality Operator:

<p>The strict inequality operator !== checks if two values are not equal and returns true if they are not equal without performing type coercion.
It returns true if the values are of different types or if they have different values.
Example:</p>

console.log(5 !== 5); // false
console.log(5 !== '5'); // true (no type coercion)
console.log(5 !== 6); // true

##### Comparison with the Greater Than Operator:

<p>The greater than (>) operator checks if the value on the left side is greater than the value on the right side.
If the value on the left side is greater than the value on the right side, the expression evaluates to true; otherwise, it evaluates to false.
Example:</p>

5 > 3; // true
3 > 5; // false
##### Comparison with the Greater Than Or Equal To Operator:

<p>The greater than or equal to (>=) operator checks if the value on the left side is greater than or equal to the value on the right side.
If the value on the left side is greater than or equal to the value on the right side, the expression evaluates to true; otherwise, it evaluates to false.
Example:</p>

5 >= 5; // true
3 >= 5; // false

##### Comparison with the Less Than Operator:

<p>The less than (&lt;) operator checks if the value on the left side is less than the value on the right side.
If the value on the left side is less than the value on the right side, the expression evaluates to true; otherwise, it evaluates to false.
Example:</p>

3 < 5; // true
5 < 3; // false

##### Comparison with the Less Than Or Equal To Operator:

<p>The less than or equal to (<=) operator checks if the value on the left side is less than or equal to the value on the right side.
If the value on the left side is less than or equal to the value on the right side, the expression evaluates to true; otherwise, it evaluates to false.
Example:</p>

3 <= 5; // true
5 <= 3; // false

##### Comparisons with the Logical And Operator:

<p>The logical AND (&&) operator returns true if both operands are true; otherwise, it returns false.
It is often used to combine multiple conditions in an if statement, where all conditions must be met for the block of code to execute.
Example:</p>

let x = 5;
let y = 10;
if (x > 0 && y > 0) {
    console.log("Both x and y are positive.");
}
##### Comparisons with the Logical Or Operator:

<p>The logical OR (||) operator returns true if at least one of the operands is true; otherwise, it returns false.
It is often used to provide alternative conditions in an if statement, where only one condition needs to be met for the block of code to execute.
Example:</p>

let x = 5;
let y = -3;
if (x > 0 || y > 0) {
    console.log("At least one of x or y is positive.");
}
<p>These comparison operators are essential for evaluating conditions in JavaScript, allowing you to control the flow of your programs based on the values of variables and other expressions.</p>


### Conditionals

#### Introducing Else Statements:

<p>In JavaScript, the else statement is used in conjunction with the if statement to execute a block of code if the condition of the if statement evaluates to false.
The else statement does not have a condition of its own. It simply executes its block of code if the preceding if statement's condition is false.
Usage:</p>

if (condition) {
    // code to execute if condition is true
} else {
    // code to execute if condition is false
}
##### Introducing Else If Statements:

<p>Sometimes, you may have multiple conditions to check in a sequence. In such cases, you can use the else if statement.
The else if statement allows you to check additional conditions if the preceding if or else if conditions evaluate to false.
Usage:</p>

if (condition1) {
    // code to execute if condition1 is true
} else if (condition2) {
    // code to execute if condition1 is false and condition2 is true
} else {
    // code to execute if all conditions are false
}
##### Logical Order in If Else Statements:

<p>In an if, else if, else statement sequence, only one block of code will be executed. The conditions are checked sequentially from top to bottom.
Once a condition evaluates to true, the corresponding block of code is executed, and the rest of the conditions are skipped.
It's important to consider the logical order of conditions to ensure that the desired behavior is achieved.</p>

###### Chaining If Else Statements:

<p>You can chain multiple if, else if, and else statements together to handle more complex decision-making scenarios.
Each if statement is evaluated independently, so even if one condition is true, subsequent conditions will still be evaluated.
Chaining if statements allows you to handle multiple conditions and execute different code blocks based on the outcome of those conditions.
Usage:</p>

if (condition1) {
    // code to execute if condition1 is true
}
if (condition2) {
    // code to execute if condition2 is true
}
// more if statements or other logic




