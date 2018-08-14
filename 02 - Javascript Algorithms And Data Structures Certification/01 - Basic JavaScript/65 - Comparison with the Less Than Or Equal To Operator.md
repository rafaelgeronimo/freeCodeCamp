# Comparison with the Less Than Or Equal To Operator

The `less than or equal to` operator (`<=`) compares the values of two numbers. If the number to the left is less than or equal to the number to the right, it returns `true`. If the number on the left is greater than the number on the right, it returns `false`. Like the equality operator, `less than or equal to` converts data types.

## Examples

```js
4 <= 5 // true
'7' <= 7 // true
5 <= 5 // true
3 <= 2 // false
'8' <= 4 // false
``` 

---

## Challenge

Add the `less than or equal to` operator to the indicated lines so that the return statements make sense.

---

## Tips

- `testLessOrEqual(0)` should return "Smaller Than or Equal to 12"

- `testLessOrEqual(11)` should return "Smaller Than or Equal to 12"

- `testLessOrEqual(12)` should return "Smaller Than or Equal to 12"

- `testLessOrEqual(23)` should return "Smaller Than or Equal to 24"

- `testLessOrEqual(24)` should return "Smaller Than or Equal to 24"

- `testLessOrEqual(25)` should return "More Than 24"

- `testLessOrEqual(55)` should return "More Than 24"

- You should use the `<=` operator at least twice

---

## Solution

```js
function testLessOrEqual(val) {
  if (val <= 12) {
    return "Smaller Than or Equal to 12";
  }  
  if (val <= 24) {
    return "Smaller Than or Equal to 24";
  }
  return "More Than 24";
}
testLessOrEqual(55);
```