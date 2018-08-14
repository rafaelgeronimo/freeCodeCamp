# Comparison with the Strict Inequality Operator

The strict inequality operator (`!==`) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns `false` where strict equality would return `true` and *vice versa*. Strict inequality will not convert data types.

## Examples

```js
3 !== 3 // false
3 !== '3' // true
4 !== 3 // true
```

---

## Challenge

Add the `strict inequality operator` to the `if` statement so the function will return "Not Equal" when `val` is not strictly equal to `17`

---

## Tips

- `testStrictNotEqual(17)` should return "Equal"

- `testStrictNotEqual("17")` should return "Not Equal"

- `testStrictNotEqual(12)` should return "Not Equal"

- `testStrictNotEqual("bob")` should return "Not Equal"

- You should use the `!==` operator

---

### Code before

```js
// Setup
function testStrictNotEqual(val) {
  // Only Change Code Below this Line
  
  if (val) {

  // Only Change Code Above this Line

    return "Not Equal";
  }
  return "Equal";
}

// Change this value to test
testStrictNotEqual(10);
```

---

## Solution

```js
// Setup
function testStrictNotEqual(val) {
  if (val !== 17) {
    return "Not Equal";
  }
  return "Equal";
}

testStrictNotEqual("bob");
```