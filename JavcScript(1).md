# <div align=center>JavaScript</div>
## What is JavaScript?
JavaScript is the Server-side & client-side Programming Language for the Web. 

JavaScript is a programming language that allows you to implement complex features on web pages.


## History: -
In 1995 Brendon created a mocha language in 10 days. Later it was called JavaScript.

In 1997 ECMAScript1 was released.

JavaScript donated to ECMA to create a standard implementation.

In 2002 Google & Yahoo started contributing to JavaScript standards And community.

JavaScript = Java+LiveScript

## Tech Debt 
1. \+ (Plus sign)  -  Use for addition & concatenation. Always do concat when one of the variables is a string.

1. === - Is used to compare values as well as data types.

1. Null – null is a primitive type but returns a typeof object


## Variable
A variable is a container and is used to store the values.

JavaScript is dynamic.

Variables are case-sensitive.

We can use _ & $ Sign to declare the variables.

CamelCase also uses to declare variables.

To identify the data type of variable we can use a predefined function typeof().

### Variable Scope
#### Local Variable
Local variables are defined within the function, and they can use in the function.

#### Global Variable
Global Variables are defined outside the function and can be accessed from anywhere.

|Var|	Let|	const|
|---|---|---|
|Can be redeclare|	As per ES6 standard let cannot be redeclared|	As per ES6 standard const cannot be redeclared|
|Can be reinitialized|	Can be reinitialized|	Can`t be reinitialized but non-primitive values can be updated|
|Functional Scope|	Lexical Scope	|Lexical Scope|
|Hoisted|	Doesn’t get hoisted|	Doesn’t get hoisted|
|ES5|	ES6|	ES6|


## Data Types: -
1.Primitive Data Type

* string:- Represents a sequence of characters e.g. “ krunal”

* number – Represent Number & Decimal values e.g. 100, 12.25

* boolean – Represents Boolean Value either true or false
*	undefined - Represents Undefined value
*	null – Represents Null Value i.e. NO value at all.  


2.Non – Primitive Data Type
* object – Represents instance through which we can access member
*	array – Represents a group of similar value

#### Falsy Value
1. NaN
1. Undefined
1. Null
1. False
1.  “ ” – Empty string
1. 0
#### Truthy Value
 
1. [] – Empty array
1. {}- Empty object
1. Other than the Falsy value, any primitive is truthy values.

## Operators:- 
#### Arithmetic Operator 
|Operator|	Description|
|:---:   |---   |
|+|	Addition|
|-|	Subtraction|
|/|	Divide|
|*|	Multiply|
|%|	Modulus|

#### Logical Operator
|Operator	|Description|
|:---:|:---|
|&& (and)	|It returns true when both conditions are true|
| \|\|( or)   |It returns true when at least one of the conditions is true|
|! ( not)	|It reverses the state of the operand|

#### Ternary Operator

The Ternary operator first evaluates an expression for a true or false value and then executes one of the two given statements depending upon the result of the evaluation.

#### Control Structure

If-else

For

Switch case

While

Do while


### Call by value: -
Primitive data types are call by value.
~~~javascript 
var a = 20;
var b = a;

a = "50";

console.log(a)
console.log(b)
~~~
~~~
output
50
20
~~~
In this example, var b copies the value of var a. When we reinitialized var a, the value of var b doesn’t change.

### Call by reference: -
Non-Primitive data types are called by reference. 
~~~javascript
var user = {name:"krunal",city:"thane"}
var result = user 
user.city = "mumbai";
console.log(user)
console.log(result)
~~~
```
output
name: "krunal",city: "mumbai"
name: "krunal",city: "mumbai"
```
In this example, var user pass the reference of its memory location to var result. If we update the object user, then the object result will also get updated.


## Function 
A Function is mainly used to reduce lines of code.

A Function is treated as object data types in JavaScript.

#### Function behavior
* Normal declaration
* Hoisting
* Override function
* Container (object)
* Scope Local & Global

##### Functional Scope: - 
A variable declared within the function can only access in the function.
#### Lexical Scope: -
A child function can access the parent function. It starts and ends with {}.


#### First-class citizen
A function can be assigned to a variable.

A function can be return from another function.

#### Function Declaration
~~~javascript
function result() {
    console.log("Hiiii");
}
result();
~~~

#### Function Expression
~~~javascript
let result = function(){
    console.log("Hiii");
}
result();
~~~
#### Higher-order function 
A function can receive the function, and a function can return the function.

#### IIFE (Immediately Invoke Function Expression)
~~~javascript
(function(){
    console.log("krunal");
})();
~~~

~~~javascript
With Parameter
(function(a,b){
    console.log("Addition of two numbers is = " +(a+b) );
})(10,20);
~~~
#### Pure function 
when the same input is passed every time, and function will return the same output.
~~~javascript
function sub(x,y){
    return(x-y)
}
let a = 20;
let b = 10;
let total = sub(a ,b)
console.log(total)
~~~

#### Arrow Function
~~~javascript
const add = (a ,b) => {
    console.log("Addition of two numbers is = "+(a+b));
}
add(10,10);
~~~

## Object 

Everything in JavaScript is an object.

An object is a non-primitive data type.

In object, data can be store as key-value pair.

~~~javaScript
let emp = {
    name: "Raj",
    age: 27,
    city: "Thane"
}
console.log(emp.name)
~~~


## Array
An array can hold multiple arguments in JavaScript.


An array is n non-primitive data type.

In an array, the default index position will always start from zero.

#### Array built-in methods
|Methods|Description|
|---|---|
|pop | is used to remove an element at the end of the array|
|push |  is used to insert an element at the end of an array|
|shift | is used to insert an element at the starting of an array|
|unshift |  is used to remove an element at the starting of an array|
|concat | is used to merge two arrays in a single array|
|indexOf |  is used to give the index position of an element|
|slice | is used to split an array|
|reverse |  is used to reverse an array|
|sort | is used to sort arrays in ascending and descending order|
|Includes | is used to check whether the element is present or not|
|isArray | is used to check whether an object is an array|


#### String built-in methods
|Methods|Description|
|---|---|
|Split | is used to split the string|
|Replace | is used to replace a specific value of the string with a new value|
|Trim | it removes the whitespace from the string|
|toLowerCase | is used to convert the string into lower case|
|toUpperCase | is used to convert the string into upper case|

#### Built in Functiuon
|Methods|Description|
|---|---|
|setTimeout | delay the code for some time|
|setInterval |  the code runs continuously|
|clearInterval |  stops the time interval|
|parseInt | it converts the string into an integer|
|parseFloat | it converts a string into a floating-point number|
