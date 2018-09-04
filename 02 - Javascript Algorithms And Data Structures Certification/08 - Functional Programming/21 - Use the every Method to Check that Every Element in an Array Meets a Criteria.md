# Use the every Method to Check that Every Element in an Array Meets a Criteria

The `every` method works with arrays to check if *every* element passes a particular test. It returns a Boolean value - `true` if all values meet the criteria, `false` if not.

For example, the following code would check if every element in the `numbers` array is less than 10:

```js
var numbers = [1, 5, 8, 0, 10, 11];
numbers.every(function(currentValue) {
  return currentValue < 10;
});
// Returns false
```

---

## Challenge

Use the `every` method inside the `checkPositive` function to check if every element in `arr` is positive. The function should return a Boolean value.

---

## Tips

- Your code should use the `every` method.

- `checkPositive([1, 2, 3, -4, 5])` should return `false`.

- `checkPositive([1, 2, 3, 4, 5])` should return `true`.

- `checkPositive([1, -2, 3, -4, 5])` should return `false`.

---

## Solution

```js
function checkPositive(arr) {
  // Add your code below this line
  return arr.every(function(currentValue) {
      return currentValue > 0;
  });
  // Add your code above this line
}
checkPositive([1, 2, 3, -4, 5]);
```