# Match Literal Strings

In the last challenge, you searched for the word `"Hello"` using the regular expression `/Hello/`. That regex searched for a literal match of the string `"Hello"`. Here's another example searching for a literal match of the string `"Kevin"`:

```js
let testStr = "Hello, my name is Kevin.";
let testRegex = /Kevin/;
testRegex.test(testStr);
// Returns true
```

Any other forms of `"Kevin"` will not match. For example, the regex `/Kevin/` will not match `"kevin"` or `"KEVIN"`.

```js
let wrongRegex = /kevin/;
wrongRegex.test(testStr);
// Returns false
```

A future challenge will show how to match those other forms as well.

---

## Challenge

Complete the regex `waldoRegex` to find `"Waldo"` in the string `waldoIsHiding` with a literal match.

---

## Tips

- Your regex `waldoRegex` should find `"Waldo"`

- Your regex `waldoRegex` should not search for anything else.

- You should perform a literal string match with your regex.

---

## Solution

```js
let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /Waldo/; // Change this line
let result = waldoRegex.test(waldoIsHiding);
```