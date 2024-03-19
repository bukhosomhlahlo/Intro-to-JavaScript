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





