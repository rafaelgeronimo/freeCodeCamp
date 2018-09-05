# Sum All Numbers in a Range

We'll pass you an array of two numbers. Return the sum of those two numbers plus the sum of all the numbers between them.

The lowest number will not always come first.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `sumAll([1, 4])` should return a number.

- `sumAll([1, 4])` should return 10.

- `sumAll([4, 1])` should return 10.

- `sumAll([5, 10])` should return 45.

- `sumAll([10, 5])` should return 45.

---

## Solution

```js
function sumAll(arr) {
  let result = 0;
  if (arr[0] > arr[1]) arr.reverse();
  for(let i = arr[0]; i <= arr[1]; i++){
    result += i;
  }
  return result;
}

sumAll([10, 5]);
```