# JavaScript Basics

![video](video-url)

This lesson covers the basics of JavaScript, the language that provides interactivity on the web.

## Variables

Variables store values that can be used and changed throughout your code.

Creating and **declaring** a variable is made up of two parts:

 1. Keywords `let` or `var`.
 1. The variable name

`let myVariable;`

`myVariable` has now been declared, but it currently doesn't have a value. Store a value in a variable with the `=` operator, followed by the expected value.

`myVariable = 123;`

`myVariable` has now been **initialized** with the value 123.

Declaration and initialization of a variable can also be condensed into one line.

`let myVariable = 123;`

Once a variable is declared, you can change its value at any point in your code with the `=` operator and the new value.

`myVariable = 321;`

## Data Types

Variables can store many different types of values, like numbers and text. These various types of values are known as the **data type**. Data types are an important part of software development because it helps developers make decisions on how the code should be written and how the software should run. Furthermore, some data types have unique features that help transform or extract additional information in a value.

### Numbers

In the previous section, the value of `myVariable` was a number data type.

`let myVariable = 123;`

Variables can store all types of numbers, including decimal or negative numbers. Numbers also can be used with arithmetic operators, covered in the [next section](#operators).

### Strings

Strings are sets of characters that reside between single or double quotes.

`'This is a string'`
`"This is also a string"`
`let myString = 'This is a string value stored in a variable';`

Remember to use quotes when writing a string, or else JavaScript will assume it's a variable name.

### Booleans

Booleans can be only two values: `true` or `false`. Booleans help make decisions on which lines of code should run when certain conditions are met. In many cases, [operators](#operators) assist with setting the value of a Boolean and you will often notice and write variables being initialized or their values being updated with an operator.

`let myTrueBool = true`
`let myFalseBool = false`

## Operators

Operators are special symbols that are used to calculate values of various data types. Most operators are mathematical symbols, but may serve another purpose other than arithmetic.

### Arithmetic Operators

Symbol | Description | Example
-- | -- | --
`+` | **Addition**: Calculates the sum of two numbers | `1 + 2 //expected answer is 3`
`-`| **Subtraction**: Calculates the difference of two numbers | `1 - 2 //expected answer is -1`
`*`| **Multiplication**: Calculates the product of two numbers | `1 * 2 //expected answer is 2`
`/` | **Division**: Calculates the quotient of two numbers | `1 / 2 //expected answer is 0.5`
`%` | **Remainder**: Calculates the remainder from the division of two numbers | `1 % 2 //expected answer is 1`

### Relational Operators

Symbol | Description | Example
-- | -- | --
`<` | **Greater than**: Compares two values and returns the `true` Boolean data type if the value on the right side is larger than the left | --
`<=`| **Greater than or equal to**: Compares two values and returns the `true` Boolean data type if the value on the right side is larger than or equal to the left | --
`>` | **Less than**: Compares two values and returns the `true` Boolean data type if the value on the left side is larger than the right | --
`=>` | **Less than or equal to**: Compares two values and returns the `true` Boolean data type if the value on the left side is larger than or equal to the right  | --

### Equality Operators

-- | -- | --
`===` | **Strict equality**: Compares two values and returns the `true` Boolean data type if values on the right and left are equal AND are the same data type. | --
`!==` | **Inequality**: Compares two values and returns the opposite Boolean value of what a strict equality operator would return  | --

## Review & Self Study

**Assignment Due [MM/YY]**: [Assignment Name](assignment.md)

Complete the following learn module(s) to complete the quiz:

[Learn Link 1]()
[Learn Link 2]()