# Steamroller

Flatten a nested array. You must account for varying levels of nesting.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `steamrollArray([[["a"]], [["b"]]])` should return `["a", "b"]`.

- `steamrollArray([1, [2], [3, [[4]]]])` should return `[1, 2, 3, 4]`.

- `steamrollArray([1, [], [3, [[4]]]])` should return `[1, 3, 4]`.

- `steamrollArray([1, {}, [3, [[4]]]])` should return `[1, {}, 3, 4]`.

---

## Solution

```js
function steamrollArray(arr) {
  // I'm a steamroller, baby
  let newArr = [].concat(...arr);
  return newArr.some(Array.isArray) ? steamrollArray(newArr) : newArr;
    //return arr;
}

//steamrollArray([1, [2], [3, [[4]]]]);
//steamrollArray([[["a"]], [["b"]]]);// should return ["a", "b"].
//steamrollArray([1, [2], [3, [[4]]]]);// should return [1, 2, 3, 4].
//steamrollArray([1, [], [3, [[4]]]]);// should return [1, 3, 4].
steamrollArray([1, {}, [3, [[4]]]]);// should return [1, {}, 3, 4].
```