# Write Arrow Functions with Parameters

Just like a normal function, you can pass arguments into arrow functions.

```js
// doubles input value and returns it
const doubler = (item) => item * 2;
```

You can pass more than one argument into arrow functions as well.

---

## Challenge

Rewrite the `myConcat` function which appends contents of `arr2` to `arr1` so that the function uses arrow function syntax.

---

## Tips

- User did replace `var` keyword.

- `myConcat` should be a constant variable (by using `const`).

- `myConcat` should be a function

- `myConcat()` returns the correct `array`

- `function` keyword was not used.

---

### Code before

```js
var myConcat = function(arr1, arr2) {
  "use strict";
  return arr1.concat(arr2);
};
// test your code
console.log(myConcat([1, 2], [3, 4, 5]));
```

---

## Solution

```js
const myConcat = (arr1, arr2) => arr1.concat(arr2);
// test your code
console.log(myConcat([1, 2], [3, 4, 5]));
```