# Passing Values to Functions with Arguments

*Parameters* are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or "*passed*") into a function when it is called are known as *arguments*.

Here is a function with two parameters, `param1` and `param2`:

```js
function testFun(param1, param2) {
  console.log(param1, param2);
}
```

Then we can call `testFun`:

```js
testFun("Hello", "World");
```

We have passed two arguments, `"Hello"` and `"World"`. Inside the function, `param1` will equal "Hello" and `param2` will equal "World". Note that you could call `testFun` again with different arguments and the parameters would take on the value of the new arguments.

---

## Challenge

1. Create a function called `functionWithArgs` that accepts two arguments and outputs their sum to the dev console.

2. Call the function with two numbers as arguments.

---

## Tips

- `functionWithArgs` should be a function

- `functionWithArgs(1,2)` should output `3`

- `functionWithArgs(7,9)` should output `16`

- Call `functionWithArgs` with two numbers after you define it.

---

### Code before

```js
// Example
function ourFunctionWithArgs(a, b) {
  console.log(a - b);
}
ourFunctionWithArgs(10, 5); // Outputs 5

// Only change code below this line.
```

---

## Solution

```js
// Example
function ourFunctionWithArgs(a, b) {
  console.log(a - b);
}
ourFunctionWithArgs(10, 5); // Outputs 5

// Only change code below this line.
function functionWithArgs(x, y) {
  console.log(x + y);
}

functionWithArgs(10,20);
```