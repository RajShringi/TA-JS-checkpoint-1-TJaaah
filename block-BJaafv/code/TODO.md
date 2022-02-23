1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

first function will return sum of a + b.
second function will log sum of a + b it does not return anything.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.  
   variable `first` will return sum of a + b. variable `second` will return undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?  
   `sum` function will add 12 and 24 and ignore 32 because there are only two parameter in sum function.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?  
   yes we can store `sum` function inside varible `add`. This type of expression is called function expression. Inside javascript function is an expression. It is a object and object is a value which we can store in a variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name) {
  return `Hello ${name}`;
}
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage(); // `Hello John'
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // alert userName 'Jhon' in alert box.

showMessage(); // 'Hello John'

alert(userName); // alert userName 'Jhon' in alert box.
```

8. What is a Anonymous Function give example of three functions.
   Anonymous function is a function which does not have any name.

```js
let add = function (a, b) {
  return a + b;
};
```

```js
let add = (a, b) => a + b;
```

```js
let add = (a, b) => {
  return a + b;
};
```

9. Can function declaration be a Anonymous Function? Explain
   yes function declaration can be anonymous function which is called anonymous function expression.

```js
let sum = function (a, b) {
  return a + b;
};
sum(3, 4); // here to call a function we need to use sum variable.
```

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

- it should show what will function will do.
- if function name is too big we should use camelcase.
- be consistent throughout the code for naming a function.
- function should have fewer arguments.
- function should do just one thing.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
