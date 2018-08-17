# Use the parseInt Function

The `parseInt()` function parses a string and returns an integer. Here's an example:

```js
var a = parseInt("007");
```

The above function converts the string "007" to an integer 7. If the first character in the string can't be converted into a number, then it returns `NaN`.

---

## Challenge

Use `parseInt()` in the `convertToInteger` function so it converts the input string `str` into an integer, and returns it.

---

## Tips

- `convertToInteger` should use the `parseInt()` function

- `convertToInteger("56")` should return a number

- `convertToInteger("56")` should return 56

- `convertToInteger("77")` should return 77

- `convertToInteger("JamesBond")` should return NaN

---

## Solution

```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");
```