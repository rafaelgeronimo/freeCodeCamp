# Falsy Bouncer

Remove all falsy values from an array.

Falsy values in JavaScript are `false`, `null`, `0`, `""`, `undefined`, and `NaN`.

Hint: Try converting each value to a Boolean.

Remember to use Read-Search-Ask if you get stuck. Write your own code.

---

## Tips

- `bouncer([7, "ate", "", false, 9])` should return `[7, "ate", 9].`

- `bouncer(["a", "b", "c"])` should return `["a", "b", "c"]`.

- `bouncer([false, null, 0, NaN, undefined, ""])` should return `[]`.

- `bouncer([1, null, NaN, 2, undefined])` should return `[1, 2]`.

---

## Solution

```js
function bouncer(arr) {
  // Don't show a false ID to this bouncer.
  let arr2 = [];
  for (let i in arr){
      let x = Boolean(arr[i]);
      if (x !== false){
          arr2.push(arr[i]);
      }
      x = "";
  }
  return arr2;
}

bouncer([7, "ate", "", false, 9]);
```