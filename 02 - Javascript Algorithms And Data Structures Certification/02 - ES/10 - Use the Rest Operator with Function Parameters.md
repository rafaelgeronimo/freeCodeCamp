# Use the Rest Operator with Function Parameters

In order to help us create more flexible functions, ES6 introduces the *rest operator* for function parameters. With the rest operator, you can create functions that take a variable number of arguments. These arguments are stored in an array that can be accessed later from inside the function.

Check out this code:

```js
function howMany(...args) {
  return "You have passed " + args.length + " arguments.";
}
console.log(howMany(0, 1, 2)); // You have passed 3 arguments
console.log(howMany("string", null, [1, 2, 3], { })); // You have passed 4 arguments.
```

The rest operator eliminates the need to check the `args` array and allows us to apply `map()`, `filter()` and `reduce()` on the parameters array.

---

## Challenge

Modify the function `sum` so that it uses the rest operator and it works in the same way with any number of parameters.

---

## Tips

- The result of `sum(0,1,2)` should be 3

- The result of `sum(1,2,3,4)` should be 10

- The result of `sum(5)` should be 5

- The result of `sum()` should be 0

- The `sum` function uses the `...` spread operator on the args parameter.

---

## Solution

```js
function sum(...args) {
    let answer = args.reduce((acc,val) => acc + val, 0);
    return answer;
}

sum();
```