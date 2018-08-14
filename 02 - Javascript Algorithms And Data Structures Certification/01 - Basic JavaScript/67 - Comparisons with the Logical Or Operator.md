# Comparisons with the Logical Or Operator

The *logical or* operator (`||`) returns `true` if either of the *operands* is `true`. Otherwise, it returns `false`.

The *logical or* operator is composed of two pipe symbols (`|`). This can typically be found between your Backspace and Enter keys.

The pattern below should look familiar from prior waypoints:

```js
if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
```

will return "Yes" only if `num` is between `5` and `10` (5 and 10 included). The same logic can be written as:

```js
if (num > 10 || num < 5) {
  return "No";
}
return "Yes";
```

---

## Challenge

Combine the two `if` statements into one statement which returns `"Outside"` if `val` is not between `10` and `20`, inclusive. Otherwise, return `"Inside"`.

---

## Tips

- You should use the `||` operator once

- You should only have one `if` statement

- `testLogicalOr(0)` should return "Outside"

- `testLogicalOr(9)` should return "Outside"

- `testLogicalOr(10)` should return "Inside"

- `testLogicalOr(15)` should return "Inside"

- `testLogicalOr(19)` should return "Inside"

- `testLogicalOr(20)` should return "Inside"

- `testLogicalOr(21)` should return "Outside"

- `testLogicalOr(25)` should return "Outside"

---

### Code before

```js
function testLogicalOr(val) {
  // Only change code below this line

  if (val) {
    return "Outside";
  }

  if (val) {
    return "Outside";
  }

  // Only change code above this line
  return "Inside";
}

// Change this value to test
testLogicalOr(15);
```

---

## Solution

```js
function testLogicalOr(val) {
  if (val < 10 || val > 20) {
    return "Outside";
  }
  return "Inside";
}
testLogicalOr(25);
```