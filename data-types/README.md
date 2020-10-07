# JavaScript Basics: Data Types

![video](video-url)

This lesson covers the basics of JavaScript, the language that provides interactivity on the web.

Let's start with variables and the data types that populate them!

## Variables

Variables store values that can be used and changed throughout your code.

Creating and **declaring** a variable is made up of two parts:

 1. Keywords `let` or `var`.
 1. The variable name

`let myVariable;`

`myVariable` has now been declared, but it currently doesn't have a value. Store a value in a variable with the `=` operator, followed by the expected value.

`myVariable = 123;`

> Note: the use of `=` in this lesson means we make use of an "assignment operator", used to set a value to a variable. It doesn't denote equality.

`myVariable` has now been **initialized** with the value 123.

Declaration and initialization of a variable can also be condensed into one line.

`let myVariable = 123;`

Once a variable is declared, you can change its value at any point in your code with the `=` operator and the new value.

`myVariable = 321;`

✅ Try it! You can write JavaScript right in your browser. Open a browser window and navigate to Developer Tools. In the console, you will find a prompt; type `let myVariable = 123`, press return, then type `myVariable`. What happens? Note, you'll learn more about these concepts in subsequent lessons.

## Constants

Constants are similar to variables, with two exceptions:

1. Constants must be initialized, or an error will occur when running code.
2. Value of a constant cannot be changed once initialized, or an error will occur when running code.

Declaration and initialization of a constant follows the same concepts as a variable, with the exception of the `const` keyword. Constants are typically declared with all uppercase letters.

`const MY_VARIABLE = 123;`

## Data Types

Variables can store many different types of values, like numbers and text. These various types of values are known as the **data type**. Data types are an important part of software development because it helps developers make decisions on how the code should be written and how the software should run. Furthermore, some data types have unique features that help transform or extract additional information in a value.

✅ Data Types are also referred to as JavaScript data primitives, as they are the lowest-level data types that are provided by the language. There are 6 primitive data types: string, number, bigint, boolean, undefined, and symbol. Take a minute to visualize what each of these primitives might represent. What is a `zebra`? How about `0`? `true`?

### Numbers

In the previous section, the value of `myVariable` was a number data type.

`let myVariable = 123;`

Variables can store all types of numbers, including decimals or negative numbers. Numbers also can be used with arithmetic operators, covered in the [next section](#operators).

### Arithmetic Operators

There are several types of operators to use when performing arithmetic functions, and some are listed here:

| Symbol | Description                                                              | Example                          |
| ------ | ------------------------------------------------------------------------ | -------------------------------- |
| `+`    | **Addition**: Calculates the sum of two numbers                          | `1 + 2 //expected answer is 3`   |
| `-`    | **Subtraction**: Calculates the difference of two numbers                | `1 - 2 //expected answer is -1`  |
| `*`    | **Multiplication**: Calculates the product of two numbers                | `1 * 2 //expected answer is 2`   |
| `/`    | **Division**: Calculates the quotient of two numbers                     | `1 / 2 //expected answer is 0.5` |
| `%`    | **Remainder**: Calculates the remainder from the division of two numbers | `1 % 2 //expected answer is 1`   |

✅ Try it! Try an arithmetic operation in your browser's console. Do the results surprise you?

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

✅ Why does `1 + 1 = 2` in JavaScript, but `'1' + '1' = 11?` Think about it. What about `'1' + 1`?

**Template literals** are another way to format strings, except instead of quotes, the backtick  is used. Anything that is not plain text must be placed inside placeholders `${ }`. This includes any variables that may be strings.

```javascript
let myString1 = "Hello";
let myString2 = "World";

`${myString1} ${myString2}!` //Hello World!
`${myString1}, ${myString2}!` //Hello World!
```

You can achieve your formatting goals with either method, but template literals will respect any spaces and line breaks.

✅ When would you use a template literal vs. a plain string?

### Booleans

Booleans can be only two values: `true` or `false`. Booleans can help make decisions on which lines of code should run when certain conditions are met. In many cases, [operators](#operators) assist with setting the value of a Boolean and you will often notice and write variables being initialized or their values being updated with an operator.

`let myTrueBool = true`
`let myFalseBool = false`

✅ A variable can be considered 'truthy' if it evaluates to a boolean `true`. Interestingly, in JavaScript, [all values are truthy unless defined as falsy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy).

🚀Challenge: JavaScript is notorious for its surprising ways of handling datatypes on occasion. Do a bit of research on these 'gotchas'. For example: case sensitivity can bite! Try this in your console: `let age = 1; let Age = 2; age == Age` (resolves `false` -- why?). What other gotchas can you find?

## Review & Self Study

Take a look at [this list of JavaScript exercises](https://css-tricks.com/snippets/javascript/) and try one. What did you learn?

**Assignment**: [Data Types Practice](assignment.md)

## [Post-lecture quiz](.github/post-lecture-quiz.md)