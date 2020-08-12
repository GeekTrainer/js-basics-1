# JavaScript Basics: Making Decisions

![video](video-url)

Making decisions and controlling the order in which your code runs makes your code reusable and robust. This section covers the syntax for controlling flow in JavaScript, and its significance when used with Boolean data types

## A Brief Recap on Booleans

Booleans can be only two values: `true` or `false`. Booleans help make decisions on which lines of code should run when certain conditions are met.

`let myTrueBool = true`
`let myFalseBool = false`

## Comparison Operators and Booleans

Operators are used to evaluate conditions by making comparisons that will create a Boolean value. The following is a list of operators that are frequently used.

Symbol | Description | Example
-- | -- | --
`<` | **Greater than**: Compares two values and returns the `true` Boolean data type if the value on the right side is larger than the left | `5 < 6 // true`
`<=`| **Greater than or equal to**: Compares two values and returns the `true` Boolean data type if the value on the right side is larger than or equal to the left | `5 <= 6 // true`
`>` | **Less than**: Compares two values and returns the `true` Boolean data type if the value on the left side is larger than the right | `5 > 6 // false`
`=>` | **Less than or equal to**: Compares two values and returns the `true` Boolean data type if the value on the left side is larger than or equal to the right  | `5 => 6 // false`
`===` | **Strict equality**: Compares two values and returns the `true` Boolean data type if values on the right and left are equal AND are the same data type. | `5 === 6 // false`
`!==` | **Inequality**: Compares two values and returns the opposite Boolean value of what a strict equality operator would return  | `5 !== 6 // true`

## If Statement

The if statement will run code in between its blocks if the condition is true.

```javascript
if (condition){

    //Condition was true. Code in this block will run.
}
```

Logical operators are often used to form the condition.

```javascript

let currentMoney  = 150;
let laptopPrice = 152.40;

if (currentMoney >= laptopPrice){

    //Condition was true. Code in this block will run.
    console.log("Getting a new laptop!");
}
```

## IF..Else Statement

The `else` statement will run the code in between its blocks when the condition is false. It's optional with an `if` statement.

```javascript
let currentMoney  = 150;
let laptopPrice = 152.40;

if (currentMoney >= laptopPrice){

    //Condition was true. Code in this block will run.
    console.log("Getting a new laptop!");
}
else{
    //Condition was true. Code in this block will run.
    console.log("Can't afford a new laptop, yet!");
}
```

## Logical Operators and Booleans

Decisions might require more than one comparison, and can be strung together with logical operators to produce a Boolean value.

Symbol | Description | Example
-- | -- | --
`&&` | **Logical AND**: Compares two Boolean expressions. Returns true **only** if both sides are true   | `(5 > 6) && (5 < 6 ) //One side is false, other is true. Returns false`
`||` | **Logical OR**: Compares two Boolean expressions. Returns true if at least one side is true | `(5 > 6) || (5 < 6) //One side is false, other is true. Returns true`
`!` | **Logical NOT**: Returns the opposite value of a Boolean expression | `!(5 > 6) // 5 is not greater than 6, but "!" will return true`

## Conditions and Decisions with Logical Operators

```javascript
let currentMoney  = 150;
let laptopPrice = 152.40;
let laptopDiscountPrice = 140;


if (currentMoney >= laptopPrice || currentMoney >= laptopDiscountPrice){

    //Condition was true. Code in this block will run.
    console.log("Getting a new laptop!");
}
else{
    //Condition was true. Code in this block will run.
    console.log("Can't afford a new laptop, yet!");
}
```

## Review & Self Study

**Assignment Due [MM/YY]**: [Assignment Name](assignment.md)

Complete the following learn module(s) to complete the quiz:

[Learn Link 1]()
[Learn Link 2]()