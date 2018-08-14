# Comparison with the Greater Than Operator

The greater than operator (`>`) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`.

Like the equality operator, greater than operator will convert data types of values while comparing.

## Examples

```js
5 > 3 // true
7 > '3' // true
2 > 3 // false
'1' > 9 // false
```

## Challenge

Add the `greater than` operator to the indicated lines so that the return statements make sense.

---

## Tips

- `testGreaterThan(0)` should return "10 or Under"

- `testGreaterThan(10)` should return "10 or Under"

- `testGreaterThan(11)` should return "Over 10"

- `testGreaterThan(99)` should return "Over 10"

- `testGreaterThan(100)` should return "Over 10"

- `testGreaterThan(101)` should return "Over 100"

- `testGreaterThan(150)` should return "Over 100"

- You should use the `>` operator at least twice

---

### Code before

```js
function testGreaterThan(val) {
  if (val) {  // Change this line
    return "Over 100";
  }
  
  if (val) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

// Change this value to test
testGreaterThan(10);
```

---

## Solution

```js
function testGreaterThan(val) {
  if (val > 100) {
    return "Over 100";
  }  
  if (val > 10) {
    return "Over 10";
  }
  return "10 or Under";
}

testGreaterThan(150);
```