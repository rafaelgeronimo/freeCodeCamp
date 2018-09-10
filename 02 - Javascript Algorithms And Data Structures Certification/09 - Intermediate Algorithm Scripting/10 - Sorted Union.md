# Sorted Union

Write a function that takes two or more arrays and returns a new array of unique values in the order of the original provided arrays.

In other words, all values present from all arrays should be included in their original order, but with no duplicates in the final array.

The unique numbers should be sorted by their original order, but the final array should not be sorted in numerical order.

Check the assertion tests for examples.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `uniteUnique([1, 3, 2], [5, 2, 1, 4], [2, 1])` should return `[1, 3, 2, 5, 4]`.

- `uniteUnique([1, 3, 2], [1, [5]], [2, [4]])` should return `[1, 3, 2, [5], [4]]`.

- `uniteUnique([1, 2, 3], [5, 2, 1])` should return `[1, 2, 3, 5]`.

- `uniteUnique([1, 2, 3], [5, 2, 1, 4], [2, 1], [6, 7, 8])` should return `[1, 2, 3, 5, 4, 6, 7, 8]`.

---

## Solution

```js
function uniteUnique(arr) {
  //console.log("Array original: " + arr);
  for (let i = 1; i < arguments.length; i++){
      //console.log("Arrays secundária(s): " + arguments[i]);
      for(let j in arguments[i]){
          if(arr.includes(arguments[i][j])){
              //console.log("O número " + arguments[i][j] + " está contido na array " + arr);
          }else{
              arr.push(arguments[i][j]);
          }
      }
  }
  return arr;
}

//uniteUnique([1, 3, 2], [5, 2, 1, 4], [2, 1]);// should return [1, 3, 2, 5, 4].
uniteUnique([1, 3, 2], [1, [5]], [2, [4]]);// should return [1, 3, 2, [5], [4]].
//uniteUnique([1, 2, 3], [5, 2, 1]);// should return [1, 2, 3, 5].
//uniteUnique([1, 2, 3], [5, 2, 1, 4], [2, 1], [6, 7, 8]);// should return [1, 2, 3, 5, 4, 6, 7, 8].
```