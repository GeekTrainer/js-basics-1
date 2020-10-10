## Functions

A function is a block of code meant to accomplish a task. You create a function by using the `function` keyword, a name, a set of parameters and function definition also known as the functions _body_. The syntax for a function looks like the following:

```javascript
function name(param, param2, param3) { // function definition
 // function definition/body
}
```

### Parameter

Parameters are listed in the definition part within parenthesis and are comma separated like so:

```javascript
(param, param2, param3)
```

### Function body

Here you define what task the function should carry out. A function may or may not return something. If a function does return something then the keyword `return` is used. The `return` keyword expects a value or reference of what's being returned like so:

```javascript
return myVariable;
```  

A more complete example can look like so:

```javascript
function add(firstValue, secondValue) {
  let sum = firstValue + secondValue;
  return sum;
}
```

In the above code the `sum` variable is being returned.

### Invocation

When you _invoke_ a function you call it with 0...N set of arguments. The argument values are then bound to the parameters corresponding to their position. The introduced `add()` method can be invoked in the following way:

```javascript
let result = add(1, 3);
console.log(result); // prints 4
```

The arguments `1` and `3` is bound to parameters `firstValue` and `secondValue` because of the order in which the parameters are defined.

JavaScript is quite flexible when it comes to invocation. You are not forced to provide arguments for all parameters, the code will run anyway. However, depending on what you pass it, the code might not behave as expected

> Challenge, try calling the `add()` method like so `add(1)` and see what happens

### Default values

There's also the concept of _default values_ on parameters. This means that if an argument is not passed to a parameter during invocation, the parameter will instead assume the default value. Consider the below code using a default value:

```javascript
function add5(firstValue, secondValue = 5) {
  return firstValue + secondValue;
}
```

Invoking the above function could look like so:

```javascript
add5(4) // returns 9
add5(4,2) // returns 6
```

Any parameters with default values must be at the end of the parameter listing. The reason is that JavaScript tries to match arguments with parameters and parameters with default values can be omitted at invocation. 
