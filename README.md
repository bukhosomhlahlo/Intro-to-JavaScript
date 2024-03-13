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





