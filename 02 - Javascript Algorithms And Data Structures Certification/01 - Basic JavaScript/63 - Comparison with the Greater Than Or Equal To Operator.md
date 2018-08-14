# Comparison with the Greater Than Or Equal To Operator

The `greater than or equal to` operator (`>=`) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns `true`. Otherwise, it returns `false`.

Like the equality operator, `greater than or equal to` operator will convert data types while comparing.

## Examples

```js
6 >= 6 // true
7 >= '3' // true
2 >= 3 // false
'7' >= 9 // false
```

---

## Challenge

Add the `greater than or equal to` operator to the indicated lines so that the return statements make sense.

---

## Tips

- `testGreaterOrEqual(0)` should return "Less than 10"

- `testGreaterOrEqual(9)` should return "Less than 10"

- `testGreaterOrEqual(10)` should return "10 or Over"

- `testGreaterOrEqual(11)` should return "10 or Over"

- `testGreaterOrEqual(19)` should return "10 or Over"

- `testGreaterOrEqual(100)` should return "20 or Over"

- `testGreaterOrEqual(21)` should return "20 or Over"

- You should use the `>=` operator at least twice

---

### Code before

```js
function testGreaterOrEqual(val) {
  if (val) {  // Change this line
    return "20 or Over";
  }
  
  if (val) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}

// Change this value to test
testGreaterOrEqual(10);
```

---

## Solution

```js
function testGreaterOrEqual(val) {
  if (val >= 20) {
    return "20 or Over";
  }  
  if (val >= 10) {
    return "10 or Over";
  }
  return "Less than 10";
}

testGreaterOrEqual(21);
```