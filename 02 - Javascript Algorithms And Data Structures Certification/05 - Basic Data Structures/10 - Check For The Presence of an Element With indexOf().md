# Check For The Presence of an Element With indexOf()

Since arrays can be changed, or *mutated*, at any time, there's no guarantee about where a particular piece of data will be on a given array, or if that element even still exists. Luckily, JavaScript provides us with another built-in method, `indexOf()`, that allows us to quickly and easily check for the presence of an element on an array. `indexOf()` takes an element as a parameter, and when called, it returns the position, or index, of that element, or `-1` if the element does not exist on the array.

For example:

```js
let fruits = ['apples', 'pears', 'oranges', 'peaches', 'pears'];

fruits.indexOf('dates') // returns -1
fruits.indexOf('oranges') // returns 2
fruits.indexOf('pears') // returns 1, the first index at which the element exists
```

## Challenge

`indexOf()` can be incredibly useful for quickly checking for the presence of an element on an array. We have defined a function, `quickCheck`, that takes an array and an element as arguments. Modify the function using `indexOf()` so that it returns `true` if the passed element exists on the array, and `false` if it does not.

---

## Tips

- `quickCheck(["squash", "onions", "shallots"], "mushrooms")` should return `false`

- `quickCheck(["squash", "onions", "shallots"], "onions")` should return `true`

- `quickCheck([3, 5, 9, 125, 45, 2], 125)` should return `true`

- `quickCheck([true, false, false], undefined)` should return `false`

- The `quickCheck` function should utilize the `indexOf()` method

---

## Solution

```js
function quickCheck(arr, elem) {
  // change code below this line
  return arr.indexOf(elem) >= 0 ? true : false;
  // change code above this line
}

// change code here to test different cases:
console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
```