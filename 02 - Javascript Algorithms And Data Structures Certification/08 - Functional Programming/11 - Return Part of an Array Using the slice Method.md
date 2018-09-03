# Return Part of an Array Using the slice Method

The `slice` method returns a copy of certain elements of an array. It can take two arguments, the first gives the index of where to begin the slice, the second is the index for where to end the slice (and it's non-inclusive). If the arguments are not provided, the default is to start at the beginning of the array through the end, which is an easy way to make a copy of the entire array. The `slice` method does not mutate the original array, but returns a new one.

Here's an example:

```js
var arr = ["Cat", "Dog", "Tiger", "Zebra"];
var newArray = arr.slice(1, 3);
// Sets newArray to ["Dog", "Tiger"]
```

---

## Challenge

Use the `slice` method in the `sliceArray` function to return part of the `anim` array given the provided `beginSlice` and `endSlice` indices. The function should return an array.

---

## Tips

- Your code should use the `slice` method.

- The `inputAnim` variable should not change.

- `sliceArray(["Cat", "Dog", "Tiger", "Zebra", "Ant"], 1, 3)` should return `["Dog", "Tiger"]`.

- `sliceArray(["Cat", "Dog", "Tiger", "Zebra", "Ant"], 0, 1)` should return `["Cat"]`.

- `sliceArray(["Cat", "Dog", "Tiger", "Zebra", "Ant"], 1, 4)` should return `["Dog", "Tiger", "Zebra"]`.

---

## Solution

```js
function sliceArray(anim, beginSlice, endSlice) {
  // Add your code below this line
  let newArr = anim.slice(beginSlice,endSlice);
  return newArr;
  // Add your code above this line
}
var inputAnim = ["Cat", "Dog", "Tiger", "Zebra", "Ant"];
sliceArray(inputAnim, 1, 3);
```