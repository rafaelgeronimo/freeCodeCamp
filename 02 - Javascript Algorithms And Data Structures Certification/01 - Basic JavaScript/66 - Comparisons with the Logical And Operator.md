# Comparisons with the Logical And Operator

Sometimes you will need to test more than one thing at a time. The *logical and* operator (`&&`) returns `true` if and only if the *operands* to the left and right of it are true.

The same effect could be achieved by nesting an if statement inside another if:

```js
if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";
```

will only return "Yes" if `num` is greater than `5` and less than `10`. The same logic can be written as:

```js
if (num > 5 && num < 10) {
  return "Yes";
}
return "No";
```

---

## Challenge

Combine the two if statements into one statement which will return `"Yes"` if `val` is less than or equal to `50` and greater than or equal to `25`. Otherwise, will return `"No"`.

---

## Tips

- You should use the `&&` operator once

- You should only have one `if` statement

- `testLogicalAnd(0)` should return "No"

- `testLogicalAnd(24)` should return "No"

- `testLogicalAnd(25)` should return "Yes"

- `testLogicalAnd(30)` should return "Yes"

- `testLogicalAnd(50)` should return "Yes"

- `testLogicalAnd(51)` should return "No"

- `testLogicalAnd(75)` should return "No"

- `testLogicalAnd(80)` should return "No"

---

### Code before

```js
function testLogicalAnd(val) {
  // Only change code below this line

  if (val) {
    if (val) {
      return "Yes";
    }
  }

  // Only change code above this line
  return "No";
}

// Change this value to test
testLogicalAnd(10);
```

---

## Solution

```js
function testLogicalAnd(val) {
  if (val >= 25 && val <= 50) {
      return "Yes";
  }
  return "No";
}
testLogicalAnd(80);
```