# Smallest Common Multiple

Find the smallest common multiple of the provided parameters that can be evenly divided by both, as well as by all sequential numbers in the range between these parameters.

The range will be an array of two numbers that will not necessarily be in numerical order.

For example, if given 1 and 3, find the smallest common multiple of both 1 and 3 that is also evenly divisible by all numbers between 1 and 3. The answer here would be 6.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `smallestCommons([1, 5])` should return a number.

- `smallestCommons([1, 5])` should return 60.

- `smallestCommons([5, 1])` should return 60.

- `smallestCommons([2, 10])` should return 2520.

- `smallestCommons([1, 13])` should return 360360.

- `smallestCommons([23, 18])` should return 6056820.

---

## Solution

```js
function smallestCommons(arr) {
  arr.sort(function(a, b) {
    return b - a;
  });

  var newArr = [];
  for (var i = arr[0]; i >= arr[1]; i--) {
    newArr.push(i);
  }
  let result = 0, loop = 1, n;

  do {
    result = newArr[0] * loop * newArr[1];
    for (n = 2; n < newArr.length; n++) {
      if (result % newArr[n] !== 0) {
        break;
      }
    }

    loop++;
  } while (n !== newArr.length);

    return result;
}

smallestCommons([2, 10]);
```