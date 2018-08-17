# Use the Conditional (Ternary) Operator

The *conditional operator*, also called the *ternary operator*, can be used as a one line if-else expression.

The syntax is:

`condition ? statement-if-true : statement-if-false;`

The following function uses an if-else statement to check a condition:

```js
function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```

This can be re-written using the `conditional operator`:

```js
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater";
}
```

---

## Challenge

Use the `conditional operator` in the `checkEqual` function to check if two numbers are equal or not. The function should return either true or false.

---

## Tips

- `checkEqual` should use the `conditional operator`

- `checkEqual(1, 2)` should return false

- `checkEqual(1, 1)` should return true

- `checkEqual(1, -1)` should return false

---

## Solution

```js
function checkEqual(a, b) {
    return a === b ? true : false;
}

checkEqual(1, 2);
```