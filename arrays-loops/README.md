# JavaScript Basics: Arrays and Loops

![video](video-url)

This lesson covers the basics of JavaScript, the language that provides interactivity on the web.

## Arrays

Working with data is a common task for any language, and it's a much easier task when data is organized in a structural format, such as arrays. With arrays, data is stored in a structure similar to a list, where each value that is stored is assigned a unique value. One major benefit of arrays is that you can store different types of data in one array.

Syntax for an array is a pair of square brackets.

`let myArray = [];`

This is an empty array, but arrays can be declared with data. Multiple values in an array are separated by a comma.

`let iceCreamFlavors = ["Chocolate", "Strawberry", "Vanilla", "Pistashio", "Rocky Road"];`

The array values are assigned a unique value called the **index**, a whole number that is assigned based on its distance from the beginning of the array. In the example above, the string value "Chocolate" has an index of 0, therefore the index of "Rocky Road" is 4. Use the index with square brackets to retrieve, change, or insert array values.

```javascript
let iceCreamFlavors = ["Chocolate", "Strawberry", "Vanilla", "Pistashio", "Rocky Road"];
iceCreamFlavors[2]; //"Vanilla"
iceCreamFlavors[4] = "Butter Pecan"; //Changed "Rocky Road" to "Butter Pecan"
iceCreamFlavors[5] = "Cookie Dough"; //Added "Cookie Dough"
```

To find out how many items are in an array by using the `length` property.

```javascript
let iceCreamFlavors = ["Chocolate", "Strawberry", "Vanilla", "Pistashio", "Rocky Road"];
iceCreamFlavors.length; //5
```

## Loops

Loops allow for repetitive or **iterative** tasks, and can save a lot of time and code. Each iteration can vary in variables, values, and conditions. There are different types of loops in JavaScript, and they have small differences that will do the same thing.

### For Loop

The `for` loop requires 3 parts to iterate:
    - `counter` A variable that is typically initialized with a number that counts the number of iterations.
    - `condition` Expression that uses comparison operators to cause the loop to stop when `true`
    - `iteration-expression` Runs at the end of each iteration, typically used to change the counter value
  
```javascript
    for (counter; condition; iteration-expression) {
    }

    //Counting up to 10
    for (let i = 0; i < 10; i++) {
        console.log(i);
    }
```

### While loop

Unlike, the syntax for the `for` loop, `while` loops only require a condition that will stop the loop when `true`. Conditions in loops usually rely on other values, like counters and must be managed during the loop. Starting values for counters must be created outside the loop, and any expressions to meet a condition, including changing the counter must be maintained inside the loop.

```javascript
while (condition) {

}

//Counting up to 10
let i = 0;
while (i < 10) {
 console.log(i);
 i++;
}

```

## Loops and Arrays

Arrays are often used with loops because most conditions require the length of the array to stop the loop, and the index can also be the counter value.

```javascript
let iceCreamFlavors = ["Chocolate", "Strawberry", "Vanilla", "Pistashio", "Rocky Road"];

for (let i = 0; i < iceCreamFlavors.length; i++) {
  console.log(iceCreamFlavors[i]);
} //Ends when all flavors are printed
```

## Review & Self Study

**Assignment Due [MM/YY]**: [Assignment Name](assignment.md)
