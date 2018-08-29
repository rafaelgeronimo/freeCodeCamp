# Finders Keepers

Create a function that looks through an array (first argument) and returns the first element in the array that passes a truth test (second argument). If no element passes the test, return undefined.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `findElement([1, 3, 5, 8, 9, 10], function(num) { return num % 2 === 0; })` should return 8.

- `findElement([1, 3, 5, 9], function(num) { return num % 2 === 0; })` should return undefined.

---

## Solution

```js
function findElement(arr, func) {
    let num;
    for(let i in arr){
        if (func(arr[i])){
        num = arr[i];
        return num;
      }
  }
  return num;
}

//findElement([1, 2, 3, 4], num => num % 2 === 0);
//findElement([1, 3, 5, 8, 9, 10], function(num) { return num % 2 === 0; });// should return 8.
findElement([1, 3, 5, 9], function(num) { return num % 2 === 0; });// should return undefined.
```