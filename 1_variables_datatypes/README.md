# JavaScript Basics: Variable and Data Types

![video](video-url)This lesson covers the basics of JavaScript, the language that provides interactivity on the web.

## Variables

Variables store values that can be used and changed throughout your code.

**Declaring** a variable is made up of two parts:

 1. Keywords `let` or `var`.
 1. The variable name

`let myVariable;`

`myVariable` has now been declared, but it's not **initialized**, which means it doesn't have a value. Initialize a variable with the `=` operator, followed by a value.

`myVariable = 123;`

`myVariable` has now been initialized with the value 123.

Declaration and initialization of a variable can also be condensed into one line.

`let myVariable = 123;`

Once a variable is declared, you can change its value at any point in your code with the `=` operator and the new value.

`myVariable = 321;`

## Constants

Constants are similar to variables, with two exceptions:

1. Constants must be initialized, or an error will occur when running code.
2. Value of a constant cannot be changed once initialized, or an error will occur when running code.

Declaration and initialization of a constant follows the same concepts as a variable, with the exception of the `const` keyword. Constants are typically declared with all uppercase letters.

`const MY_VARIABLE = 123;`

## Data Types

Variables can store many different types of values, like numbers and text. These various types of values are known as the **data type**. Data types are an important part of software development because it helps developers make decisions on how the code should be written and how the software should run. Furthermore, some data types have unique features that help transform or extract additional information in a value.

### Numbers

In the previous section, the value of `myVariable` was a number data type.

`let myVariable = 123;`

Variables can store all types of numbers, including decimal (also known as floats) or negative numbers.

### Basic Math

Basic math can be done on any type of number data type. The following are symbols reserved in JavaScript for basic arithmetic, followed by examples of use.

Symbol | Description | Example
-- | -- | --
`+` | **Addition**: Calculates the sum of two numbers | `1 + 2 //expected answer is 3`
`-`| **Subtraction**: Calculates the difference of two numbers | `1 - 2 //expected answer is -1`
`*`| **Multiplication**: Calculates the product of two numbers | `1 * 2 //expected answer is 2`
`/` | **Division**: Calculates the quotient of two numbers | `1 / 2 //expected answer is 0.5`
`%` | **Remainder**: Calculates the remainder from the division of two numbers | `1 % 2 //expected answer is 1`

### Strings

Strings are sets of characters that reside between single or double quotes.

`'This is a string'`
`"This is also a string"`
`let myString = 'This is a string value stored in a variable';`

Remember to use quotes when writing a string, or else JavaScript will assume it's a variable name.

### Formatting Strings

Strings are textual, and will require formatting from time to time.

To **concatenate** two or more strings, or join them together, use the `+` operator.

```javascript
let myString1 = "Hello";
let myString2 = "World";

myString1 + myString2 + "!"; //HelloWorld!
myString1 + " " + myString2 + "!"; //Hello World!
myString1 + ", " + myString2 + "!"; //Hello, World!

```

**Template literals** are another way to format strings, except instead of quotes, the backtick is used. Anything that is not plain text must be placed inside placeholders `${ }`. This includes any variables that may be strings.

```javascript
let myString1 = "Hello";
let myString2 = "World";

`${myString1} ${myString2}!` //Hello World!
`${myString1}, ${myString2}!` //Hello World!
```

You can achieve your formatting goals with either method, but template literals will respect any spaces and line breaks.

### Booleans

Booleans can be only two values: `true` or `false`. Booleans help make decisions on which lines of code should run when certain conditions are met.

`let myTrueBool = true`
`let myFalseBool = false`

## Review & Self Study

**Assignment Due [MM/YY]**: [Assignment Name](assignment.md)

Complete the following learn module(s) to complete the quiz:

[Learn Link 1]()
[Learn Link 2]()