# Day 1
## Variables, Operators & Assignments
### Variables
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

<h1>Week 2</h1>
<h1>Day 1</h1>
<h2>Introduction to HTML, CSS and Javascript</h2>
<h3>Type Conversions</h3>


##### String Conversion:

<p>Any value in JavaScript can be converted to a string using the String() function or by using the toString() method available on most objects.</p>
let value = true; 
alert(typeof value); // boolean  
value = String(value); // now value is a string "true"  
alert(typeof value); // string  

##### Numeric Conversion:
Values in JavaScript can be converted to numbers using the Number() function or by using the unary plus (+) operator.
If the conversion is not possible, JavaScript will return NaN (Not a Number).
For example:

let str = "123";
alert(typeof str); //  string
let num = Number(str); // becomes a number 123  
alert(typeof num); // number 

OR

Number("123");  // 123
+"123";  // 123
Number("hello");  // NaN

##### Numeric conversion rules:  

 <table><tr><th>Value</th><th>Becomes</th></tr><tr><td>undefined </td><td>NaN</td></tr><tr><td>Null</td><td>0</td></tr><tr><td>true and false</td><td>1 and 0</td></tr><tr><td>string</td><td>Whitespaces from the start and end are removed. If the remaining string is empty, the result is 0. Otherwise, the number is “read” from the string. An error gives NaN.  </td></tr></table>

<p>Examples:</p> 

alert( Number("123") ); // 123  
alert( Number("123z") ); // NaN (error reading a number at "z")  
alert( Number(true) );  // 1  
alert( Number(false) );  // 0 

##### Boolean conversion:


<p>Values in JavaScript can be converted to booleans using the Boolean() function or by using the double negation (!!) operator.
Any value that is considered "falsy" (e.g., 0, "", null, undefined, NaN) will be converted to false. All other values will be converted to true.</p>
For example:

Boolean(123);  // true
!!0;  // false

alert( Boolean(0) ); // false 
alert( Boolean("hello") ); // true  
alert( Boolean("") ); // false  
alert( Boolean(1) ); // true 

##### Formatting Numbers
<p>When choosing a method for formatting numbers in JavaScript, consider factors such as locale requirements, precision, performance, and the level of customization needed. Use built-in methods for basic formatting tasks and consider third-party libraries for more advanced scenarios.</p>

<table><tr><th>Method</th><th>Description</th></tr><tr><td>Number()</td><td>Return number converted from its argument</td></tr><tr><td>parseFloat()</td><td>parse its argument and return a float</td></tr><tr><td>parseInt()</td><td>Parse its argument and returns an integer</td></tr></table>

<i>However, some JavaScript number format methods are specifically used on numbers only.</i>  

<table><tr><th>Method</th><th>Description</th></tr><tr><td>toString()</td><td>Return number as string</td></tr><tr><td>toExponential</td><td>Return string with number rounded and written with exponential notation.</td></tr><tr><td>toFixed</td><td>Return string with number rounded and written using a specified number of decimals.</td></tr><tr><td>toPrecision</td><td>Return string with a number written with a specified length</td></tr><tr><td>valueOf</td><td>Return number as a number.</td></tr></table>

A JavaScript object refers to any HTML element within a document that can be accessed through JavaScript. This includes not only HTML elements but also the browser window itself, which is also scriptable.

Apart from HTML elements, there exist core objects outside the scope of a web page, associated directly with the JavaScript language. Additionally, homemade objects are defined within the JavaScript Object Model alongside core objects. Examples of JavaScript objects include 'window', 'document', 'form', and 'image'.

Properties represent characteristics of objects. They are akin to HTML tag attributes. However, a key difference is that JavaScript properties can also be objects themselves. For instance, a document, a form, or an image, though properties of the window or document object, are considered objects in their own right if they possess their own properties and methods.

Methods are actions applicable directly to objects. In the context of a web page, methods allow for interactive experiences, enhancing user engagement. Methods are denoted by parentheses following their names, with parameters sometimes required to execute specific tasks.

Some common JavaScript methods include 'alert()', 'write()', and 'focus()'. These methods perform actions such as displaying alerts, writing content to a page, and inserting the mouse cursor into a form element.

The DOM (Document Object Model) encompasses APIs (Application Programming Interfaces) for web and XML page scripting. The 'document' and 'window' objects are frequently utilized in DOM programming. The 'window' object represents the browser environment, while the 'document' object serves as the root of the document. Together with the 'Element' interface, these objects offer methods and properties for working with individual elements on a page.

Path references in JavaScript code typically include the 'document' object, given that most objects within a web page are contained within it. However, since the 'document' is contained by the 'window' object, references to the 'window' object are often omitted. This is due to the assumption that methods invoked without specifying the object are intended for the 'window' object, which sits at the top of the object hierarchy.

In summary, the DOM structure involves various objects, properties, and methods that enable interaction and manipulation of web content through JavaScript.

## Day 2

### Javascript APIS
<p>These are common APIs (Application Programming Interfaces) in web and XML page scripting using the DOM (Document Object Model)</p>

1. `document.getElementById(id)`:
   - This method retrieves an HTML element with the specified 'id' attribute from the current document.

2. `document.getElementsByTagName(name)`:
   - This method retrieves a collection of HTML elements with the specified tag name from the current document.

3. `document.createElement(name)`:
   - This method creates a new HTML element with the specified tag name.

4. `parentNode.appendChild(node)`:
   - This method appends a new child node to the end of the list of children of a specified parent node.

5. `element.innerHTML`:
   - This property represents the HTML content (including child elements) of an element.

6. `element.style.left`:
   - This property sets or returns the left position of a positioned element.

7. `element.setAttribute`:
   - This method sets the value of an attribute on the specified element.

8. `element.getAttribute`:
   - This method retrieves the value of the specified attribute on the given element.

9. `element.addEventListener`:
   - This method attaches an event handler to the specified element, allowing the execution of a specified function when a particular event occurs.

10. `window._content`:
    - This property represents the content area of the browser window.

11. `window.onload`:
    - This event occurs when the DOM (Document Object Model) has been fully loaded in the current window.

12. `window.dump()`:
    - This method displays a message in the JavaScript console or debugging output.

13. `window.scrollTo()`:
    - This method scrolls the document to a specified set of coordinates (x, y) within the window.

These APIs are essential for manipulating and interacting with HTML elements and documents dynamically using JavaScript. They enable developers to access, create, modify, and handle various aspects of web pages and their content programmatically.

##### Calling one function from another function

<p>Calling one function from another function is a common practice in programming and can be done in various programming languages, including JavaScript.</p>

Here's a basic example in JavaScript:

function firstFunction() {
    console.log("This is the first function.");
    
    // Call the second function
    secondFunction();
}

function secondFunction() {
    console.log("This is the second function.");
}

// Call the first function to start the sequence
firstFunction();


In this example:

We have two functions: firstFunction() and secondFunction().
Inside firstFunction(), we call secondFunction() by simply using its name followed by parentheses. This triggers the execution of the secondFunction() code.
When the firstFunction() is called at the end of the script, it starts the sequence of function calls, which includes calling secondFunction().

The output will be:


This is the first function.
This is the second function.


##### Creating pbjects with user-defined functions

In JavaScript, you can create objects using user-defined functions. These functions act as constructors for the objects.

// Define a constructor function for creating Person objects
function Person(name, age) {
    this.name = name; // 'this' refers to the current object being created
    this.age = age;
    
    // Define a method for the Person object
    this.greet = function() {
        console.log("Hello, my name is " + this.name + " and I am " + this.age + " years old.");
    };
}

// Create instances of Person objects using the constructor function
var person1 = new Person("Alice", 30);
var person2 = new Person("Bob", 25);

// Access properties and call methods of the created objects
console.log(person1.name); // Output: Alice
console.log(person2.age); // Output: 25
person1.greet(); // Output: Hello, my name is Alice and I am 30 years old.
person2.greet(); // Output: Hello, my name is Bob and I am 25 years old.


In this example:

We define a constructor function called Person which takes name and age parameters.
Inside the constructor function, we use the this keyword to refer to the current object being created. We assign values to properties (name and age) of the object using this.
We also define a method greet() within the constructor function, which is added to each object created by the constructor.
We create two instances of Person objects using the new keyword followed by the constructor function name and passing arguments for name and age.
We access the properties (name and age) and call the method greet() of the created objects.
This demonstrates how you can create objects with user-defined functions (constructors) in JavaScript. It's a foundational concept in object-oriented programming with JavaScript.

##### Defining new properties to already-made objects

In JavaScript, you can add new properties to already-existing objects even after they have been created. :


// Define an object
var person = {
    name: "Alice",
    age: 30
};

// Add a new property to the object
person.city = "New York";

// Add a new method to the object
person.greet = function() {
    console.log("Hello, my name is " + this.name + " and I am from " + this.city + ".");
};

// Access and use the properties and method of the modified object
console.log(person.name); // Output: Alice
console.log(person.city); // Output: New York
person.greet(); // Output: Hello, my name is Alice and I am from New York.

In this example:

We have an object named person with properties name and age.
We add a new property city to the person object by simply assigning a value to it.
We also add a new method greet to the person object by assigning a function to it.
We can then access the newly added property city and call the newly added method greet.
This demonstrates how you can define new properties and methods to already-made objects in JavaScript, allowing you to dynamically extend the capabilities of objects in our code.

##### Defining properties when you create the object

In JavaScript, you can define properties for an object when you create it using either object literal notation or constructor functions. 

Here are examples of both approaches:

###### Object Literal Notation:

// Define an object with properties
var person = {
    name: "Alice",
    age: 30,
    city: "New York",
    greet: function() {
        console.log("Hello, my name is " + this.name + " and I am from " + this.city + ".");
    }
};

// Access and use the properties and method of the object
console.log(person.name); // Output: Alice
console.log(person.city); // Output: New York
person.greet(); // Output: Hello, my name is Alice and I am from New York.

###### Constructor Functions:

// Define a constructor function for creating Person objects
function Person(name, age, city) {
    this.name = name;
    this.age = age;
    this.city = city;
    
    this.greet = function() {
        console.log("Hello, my name is " + this.name + " and I am from " + this.city + ".");
    };
}

// Create an instance of the Person object using the constructor function
var person = new Person("Alice", 30, "New York");

// Access and use the properties and method of the object
console.log(person.name); // Output: Alice
console.log(person.city); // Output: New York
person.greet(); // Output: Hello, my name is Alice and I am from New York.

In both examples:

We define properties (name, age, city) for the object when creating it.
In the first example, we directly create the object using object literal notation.
In the second example, we define a constructor function Person to create Person objects with specified properties and a method.
These approaches allow us to define properties for objects at the time of object creation in JavaScript.

##### Comparison operators



Comparison operators in JavaScript are used to compare values and determine the relationship between them. Here's a list of comparison operators in JavaScript:

Equal to (==): Compares whether two values are equal. It performs type coercion, so it may convert the operands to the same type before making the comparison.


console.log(5 == 5); // Output: true
console.log(5 == '5'); // Output: true (Type coercion)
console.log(5 == 6); // Output: false

Strict equal to (===): Compares whether two values are equal and of the same type.


console.log(5 === 5); // Output: true
console.log(5 === '5'); // Output: false (Type mismatch)

Not equal to (!=): Compares whether two values are not equal. It performs type coercion.


console.log(5 != 6); // Output: true
console.log(5 != '5'); // Output: false (Type coercion)

Strict not equal to (!==): Compares whether two values are not equal or of the same type.


console.log(5 !== '5'); // Output: true
console.log(5 !== 5); // Output: false (Type match)
Greater than (>): Checks if the left operand is greater than the right operand.


console.log(5 > 3); // Output: true
console.log(5 > 5); // Output: false

Greater than or equal to (>=): Checks if the left operand is greater than or equal to the right operand.


console.log(5 >= 5); // Output: true
console.log(5 >= 3); // Output: true

Less than (<): Checks if the left operand is less than the right operand.


console.log(3 < 5); // Output: true
console.log(5 < 5); // Output: false

Less than or equal to (<=): Checks if the left operand is less than or equal to the right operand.


console.log(5 <= 5); // Output: true
console.log(3 <= 5); // Output: true

These comparison operators are fundamental for creating conditions and controlling the flow of program execution in JavaScript.

##### Arithmetic operators

Arithmetic operators in JavaScript are used to perform mathematical operations on numeric values. Here's a list of arithmetic operators in JavaScript:

Addition (+): Adds two operands.

console.log(5 + 3); // Output: 8

Subtraction (-): Subtracts the right operand from the left operand.
console.log(5 - 3); // Output: 2

Multiplication (*): Multiplies two operands.
console.log(5 * 3); // Output: 15

Division (/): Divides the left operand by the right operand.
console.log(6 / 2); // Output: 3

Modulus (%): Returns the remainder of the division operation.
console.log(10 % 3); // Output: 1

Increment (++): Increases the value of a variable by 1.
let x = 5;
x++;
console.log(x); // Output: 6

Decrement (--): Decreases the value of a variable by 1.
let y = 5;
y--;
console.log(y); // Output: 4

Exponentiation ()**: Raises the left operand to the power of the right operand.
console.log(2 ** 3); // Output: 8 (2 raised to the power of 3)

##### Bitwise Operators

These arithmetic operators are fundamental for performing calculations in JavaScript, and they follow the standard rules of arithmetic.

Bitwise operators in JavaScript are used to perform bitwise operations on integer operands. These operations treat the operands as a sequence of bits (binary digits). Here's a list of bitwise operators in JavaScript:

Bitwise AND (&): Performs a bitwise AND operation on each pair of corresponding bits. The result is 1 if both bits are 1, otherwise 0.
console.log(5 & 3); // Output: 1 (binary: 101 & 011 = 001)

Bitwise OR (|): Performs a bitwise OR operation on each pair of corresponding bits. The result is 1 if at least one of the bits is 1.
console.log(5 | 3); // Output: 7 (binary: 101 | 011 = 111)

Bitwise XOR (^): Performs a bitwise XOR (exclusive OR) operation on each pair of corresponding bits. The result is 1 if the bits are different, otherwise 0.
console.log(5 ^ 3); // Output: 6 (binary: 101 ^ 011 = 110)

Bitwise NOT (~): Performs a bitwise NOT operation on each bit, inverting its value. It turns 0 into 1 and 1 into 0. Note that it operates on each bit individually, and it flips all bits including the sign bit.
console.log(~5); // Output: -6 (binary: ~0101 = 1010, in two's complement representation -1010 = -6)

Left Shift (<<): Shifts the bits of the left operand to the left by a specified number of positions. Zeroes are shifted in from the right.
console.log(5 << 1); // Output: 10 (binary: 101 << 1 = 1010)

Sign-propagating Right Shift (>>): Shifts the bits of the left operand to the right by a specified number of positions. The sign bit is used to fill the leftmost positions.
console.log(5 >> 1); // Output: 2 (binary: 101 >> 1 = 10)

Zero-fill Right Shift (>>>): Shifts the bits of the left operand to the right by a specified number of positions. Zeroes are shifted in from the left, and the sign bit is ignored.
console.log(-5 >>> 1); // Output: 2147483645 (binary: 11111111111111111111111111111011 >>> 1 = 01111111111111111111111111111101)

These bitwise operators are used in scenarios where manipulation of individual bits is necessary, such as low-level programming, cryptography, and optimization. They are particularly useful when working with binary data and bitwise flags.

Bitwise operators in JavaScript are used to perform bitwise operations on integer operands. These operations treat the operands as a sequence of bits (binary digits). Here's a list of bitwise operators in JavaScript:

Bitwise AND (&): Performs a bitwise AND operation on each pair of corresponding bits. The result is 1 if both bits are 1, otherwise 0.


console.log(5 & 3); // Output: 1 (binary: 101 & 011 = 001)
Bitwise OR (|): Performs a bitwise OR operation on each pair of corresponding bits. The result is 1 if at least one of the bits is 1.


console.log(5 | 3); // Output: 7 (binary: 101 | 011 = 111)
Bitwise XOR (^): Performs a bitwise XOR (exclusive OR) operation on each pair of corresponding bits. The result is 1 if the bits are different, otherwise 0.


console.log(5 ^ 3); // Output: 6 (binary: 101 ^ 011 = 110)
Bitwise NOT (~): Performs a bitwise NOT operation on each bit, inverting its value. It turns 0 into 1 and 1 into 0. Note that it operates on each bit individually, and it flips all bits including the sign bit.


console.log(~5); // Output: -6 (binary: ~0101 = 1010, in two's complement representation -1010 = -6)
Left Shift (<<): Shifts the bits of the left operand to the left by a specified number of positions. Zeroes are shifted in from the right.


console.log(5 << 1); // Output: 10 (binary: 101 << 1 = 1010)
Sign-propagating Right Shift (>>): Shifts the bits of the left operand to the right by a specified number of positions. The sign bit is used to fill the leftmost positions.


console.log(5 >> 1); // Output: 2 (binary: 101 >> 1 = 10)
Zero-fill Right Shift (>>>): Shifts the bits of the left operand to the right by a specified number of positions. Zeroes are shifted in from the left, and the sign bit is ignored.


console.log(-5 >>> 1); // Output: 2147483645 (binary: 11111111111111111111111111111011 >>> 1 = 01111111111111111111111111111101)
These bitwise operators are used in scenarios where manipulation of individual bits is necessary, such as low-level programming, cryptography, and optimization. They are particularly useful when working with binary data and bitwise flags.

![image](https://github.com/bukhosomhlahlo/Intro-to-JavaScript/assets/159022974/95107d6f-48f2-41c0-b75e-20226051b9f1)

### The Document Object Model

Event Propagation
handleCheck = e => { 

  e.stopPropagation() 

  // talk to my API, set the record as "done" or not 

} 

<span onClick={this.handleCheck}>[]</span> 

That e.stopPropagation() halts this “bubbling” of events “up” through the DOM. We stop all the events from the parents occurring.


##### Event Deligation

Event delegation is a technique in JavaScript where instead of attaching an event handler to each individual element, you attach a single event handler to a parent element. This handler then listens for events bubbling up from child elements. Event delegation is particularly useful when you have a large number of elements that need the same event handling logic, or when elements are dynamically added or removed from the DOM.


Attach Event Listener to Parent Element: You attach an event listener to a parent element that contains the child elements you want to target.

Event Bubbling: When an event occurs on a child element, it bubbles up through its ancestors, triggering event handlers on each ancestor element.

Check Event Target: In the event handler attached to the parent element, you check the event.target property to determine which specific child element triggered the event.

Perform Action: Based on the event.target, you perform the desired action.


<ul id="parentList">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>

<script>
    // Attach event listener to parent element
    document.getElementById('parentList').addEventListener('click', function(event) {
        // Check if the clicked element is an <li> element
        if (event.target.tagName === 'LI') {
            // Perform action (e.g., toggle class)
            event.target.classList.toggle('highlight');
        }
    });
</script>
In this example:

<ul><li>We attach a click event listener to the &lt;ul&gt; element with the id parentList.</li>
<li>When a click event occurs on any &lt;li&gt element within the &lt;ul&gt, the event bubbles up to the &lt;ul&gt; element, triggering the event handler.</li>
<li>We check if the clicked element (event.target) is an &lt;li&gt; element.</li>
<li>If it is, we perform an action, such as toggling a class.,</li></ul>
  
Event delegation reduces the number of event handlers needed, resulting in cleaner and more efficient code, especially in scenarios where elements are dynamically added or removed. It also simplifies the management of event handling logic for multiple elements.

In JavaScript, you can use regular expressions (regex) with methods like match(), test(), search(), replace(), and split() to perform various operations on strings. When it comes to finding items in a webpage using regular expressions, you typically use them in combination with methods like querySelectorAll() or getElementsByTagName() to select elements from the DOM and then apply regex to the content of those elements.

# Day 3
## JavaScript Forms
In JavaScript, methods are functions that are defined within objects and are invoked on those objects. The this keyword is used within methods to refer to the current object the method is being called on. Understanding how methods work with the this keyword is essential for object-oriented programming in JavaScript. Here's an explanation of JavaScript methods and the this keyword:

#### Methods in JavaScript:
<p>Definition: Methods are functions that are associated with objects. They are defined within the context of an object and can access the object's properties and other methods.</p>.

Syntax:

const object = {

    property1: value1,
    
    property2: value2,
    
    methodName: function() {
    
        // Method body
    }
};

Invocation: Methods are invoked using dot notation (object.methodName()) or bracket notation (object['methodName']()).

The "this" Keyword:
Definition: The this keyword refers to the current object context within which a function is called. It dynamically points to different objects depending on how the function is called.

Usage: Inside a method, this refers to the object on which the method is being invoked.

Example:

const person = {

    name: 'Alice',
    
    greet: function() {
    
        console.log('Hello, my name is ' + this.name);
        
    }
};
person.greet(); // Output: Hello, my name is Alice

Binding: The value of this is determined by how a function is called, not where it is defined. It can be explicitly bound to a specific object using methods like call(), apply(), or bind().

#### Using this in Methods:

Accessing Object Properties: Inside a method, this allows access to the object's properties and other methods.

Modifying Object State: Methods can use this to modify the state of the object they belong to.

Dynamic Context: The value of this is determined dynamically at runtime based on how the method is called, allowing for flexible and reusable code.

Understanding JavaScript methods and the this keyword is crucial for creating object-oriented code and leveraging the power of objects in JavaScript programming.

##### Java Email Validation

Validating email addresses in JavaScript typically involves using regular expressions to match the pattern of a valid email address. While a perfect email validation regex is complex due to the intricacies of the email specification, a basic regex pattern can cover most common cases. Here's an example of how you can perform email validation in JavaScript:


function validateEmail(email) {

    // Regular expression pattern for basic email validation
    const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    
    // Test the email against the regex pattern
    return regex.test(email);
}

// Example usage:
const email1 = 'user@example.com';
const email2 = 'invalid.email@';

console.log(validateEmail(email1)); // Output: true
console.log(validateEmail(email2)); // Output: false


The regular expression /^[^\s@]+@[^\s@]+\.[^\s@]+$/ is used for validating email addresses in JavaScript. Let's break down the meaning of each part:

^: Asserts the start of the string.

[^\s@]+: Matches one or more characters that are not whitespace (\s) or @. This part represents the local part of the email address before the @ symbol.

@: Matches the @ symbol.

[^\s@]+: Matches one or more characters that are not whitespace (\s) or @. This part represents the domain name of the email address after the @ symbol.

\.: Matches a literal dot (.). It's escaped with a backslash because dot (.) has a special meaning in regular expressions and needs to be treated as a literal dot.

[^\s@]+: Matches one or more characters that are not whitespace (\s) or @. This part represents the top-level domain (TLD) of the email address.

$: Asserts the end of the string.

Putting it all together, the regular expression ensures that:

The email address starts with one or more characters that are not whitespace or @.
Followed by an @ symbol.
Followed by one or more characters that are not whitespace or @.
Followed by a dot (.).
Followed by one or more characters that are not whitespace or @.
Ends with the end of the string.
This regular expression provides a basic validation for email addresses. However, it's important to note that email address validation can be quite complex due to the variety of valid email formats and internationalization considerations. This regex does not cover all edge cases and may need to be adjusted based on specific requirements.

# Week 3
## Handling Events
### String Operations

##### Accessing Individual Characters in a String:
You can access individual characters in a string using bracket notation ([]) or the charAt() method.

Using Bracket Notation:

const str = "Hello";

// Accessing the first character
const firstChar = str[0];
console.log(firstChar); // Output: "H"

// Accessing the third character
const thirdChar = str[2];
console.log(thirdChar); // Output: "l"
Using charAt() Method:

const str = "Hello";

// Accessing the first character
const firstChar = str.charAt(0);
console.log(firstChar); // Output: "H"

// Accessing the third character
const thirdChar = str.charAt(2);
console.log(thirdChar); // Output: "l"
Comparing Strings:
You can compare strings in JavaScript using comparison operators (==, ===, !=, !==, <, >, <=, >=) or methods like localeCompare().

Using Comparison Operators:

const str1 = "apple";
const str2 = "banana";

console.log(str1 === str2); // Output: false
console.log(str1 < str2); // Output: true (lexicographic comparison)
Using localeCompare() Method:

const str1 = "apple";
const str2 = "banana";

console.log(str1.localeCompare(str2)); // Output: -1 (str1 comes before str2)
When using localeCompare(), it returns:

-1 if the first string comes before the second string alphabetically.
0 if the strings are equal.
1 if the first string comes after the second string alphabetically.
These are basic examples of how you can access individual characters in a string and compare strings in JavaScript. String manipulation and comparison are common tasks in JavaScript programming, and understanding these operations is essential for working with text data effectively.

#### Event Handlers


<p>JavaScript event handlers are functions that are invoked in response to specific events occurring in the browser. These events can be triggered by user actions (such as clicks, key presses, mouse movements) or by the browser itself (such as page loading, form submission, etc.). Event handlers allow you to define custom behavior for these events, enabling interactive and dynamic web applications.</p>

There are different ways to attach event handlers to HTML elements in JavaScript:

##### Inline Event Handlers

You can specify event handlers directly within HTML elements using the on prefix followed by the event name as an attribute. For example:


<button onclick="handleClick()">Click me</button>
In this example, the handleClick() function will be called when the button is clicked.

##### DOM Event Handlers

You can use the DOM (Document Object Model) API to attach event handlers programmatically. This method provides more flexibility and separation of concerns compared to inline event handlers. For example:


<button id="myButton">Click me</button>

const button = document.getElementById('myButton');
button.addEventListener('click', handleClick);

function handleClick() {
    // Event handling logic
}
Here, we use addEventListener() to add a click event listener to the button element. When the button is clicked, the handleClick() function will be invoked.

Event Delegation: With event delegation, you attach a single event handler to a parent element, which will then handle events for its child elements. This is particularly useful when you have a large number of elements or dynamically generated content. For example:


<ul id="myList">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>

const list = document.getElementById('myList');
list.addEventListener('click', handleClick);

function handleClick(event) {
    if (event.target.tagName === 'LI') {
        // Event handling logic
    }
}
Here, we attach a click event listener to the <ul> element, and the handleClick() function is called when any <li> element inside the list is clicked. We then check if the clicked element is an <li> before performing any action.
Event handlers play a crucial role in building interactive web applications, allowing you to respond to user actions and create dynamic user experiences.

<table><tr><th>Attribute</th></tr><tr><th>Description</th></tr></table>

















