# Seek and Destroy

You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.

**Note**
You have to use the `arguments` object.

Remember to use Read-Search-Ask if you get stuck. Write your own code.

---

## Tips

- `destroyer([1, 2, 3, 1, 2, 3], 2, 3)` should return `[1, 1]`.

- `destroyer([1, 2, 3, 5, 1, 2, 3], 2, 3)` should return `[1, 5, 1]`.

- `destroyer([3, 5, 1, 2, 2], 2, 3, 5)` should return `[1]`.

- `destroyer([2, 3, 2, 3], 2, 3)` should return `[]`.

- `destroyer(["tree", "hamburger", 53], "tree", 53)` should return `["hamburger"]`.

- `destroyer(["possum", "trollo", 12, "safari", "hotdog", 92, 65, "grandma", "bugati", "trojan", "yacht"], "yacht", "possum", "trollo", "safari", "hotdog", "grandma", "bugati", "trojan")` should return `[12,92,65]`.

---

## Solution

```js
function destroyer(arr) {
  // Remove all the values
    let args = [...arguments];
    args.splice(0,1);
    return arr.filter(function (val){
        return args.indexOf(val) === -1;
    });
}

//destroyer([1, 2, 3, 1, 2, 3], 2, 3);
//destroyer([1, 2, 3, 5, 1, 2, 3], 2, 3);
//destroyer([3, 5, 1, 2, 2], 2, 3, 5);
destroyer([2, 3, 2, 3], 2, 3);
```