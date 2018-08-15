# Returning Boolean Values from Functions

You may recall from [Comparison with the Equality Operator](https://learn.freecodecamp.org/waypoint-comparison-with-the-equality-operator) that all comparison operators return a boolean `true` or `false` value.

Sometimes people use an if/else statement to do a comparison, like this:

```js
function isEqual(a,b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
```

But there's a better way to do this. Since `===` returns `true` or `false`, we can return the result of the comparison:

```js
function isEqual(a,b) {
  return a === b;
}
```

---

## Challenge

Fix the function `isLess` to remove the `if/else` statements.

---

## Tips

- `isLess(10,15)` should return true

- `isLess(15,10)` should return false

- You should not use any `if` or `else` statements

---

### Code before

```js
function isLess(a, b) {
  // Fix this code
  if (a < b) {
    return true;
  } else {
    return false;
  }
}

// Change these values to test
isLess(10, 15);
```

---

## Solution

```js
function isLess(a, b) {
  return a < b;
}
isLess(10, 15);
```