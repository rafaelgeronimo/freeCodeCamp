# Generate Random Fractions with JavaScript

Random numbers are useful for creating random behavior.

JavaScript has a `Math.random()` function that generates a random decimal number between `0` (inclusive) and not quite up to `1` (exclusive). Thus `Math.random()` can return a `0` but never quite return a `1`

## Note

Like [Storing Values with the Equal Operator](https://learn.freecodecamp.org/storing-values-with-the-assignment-operator), all function calls will be resolved before the `return` executes, so we can `return` the value of the `Math.random()` function.

---

## Challenge

Change `randomFraction` to return a random number instead of returning `0`.

---

## Tips

- `randomFraction` should return a random number.

- The number returned by `randomFraction` should be a decimal.

- You should be using `Math.random` to generate the random decimal number.

---

## Solution

```js
function randomFraction() {

  // Only change code below this line.

    return Math.random();

  // Only change code above this line.
}
```