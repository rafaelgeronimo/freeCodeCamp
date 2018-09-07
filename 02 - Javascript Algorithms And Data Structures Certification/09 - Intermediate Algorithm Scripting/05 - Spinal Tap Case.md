# Spinal Tap Case

Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `spinalCase("This Is Spinal Tap")` should return `"this-is-spinal-tap"`.

- `spinalCase("thisIsSpinalTap")` should return `"this-is-spinal-tap"`.

- `spinalCase("The_Andy_Griffith_Show")` should return `"the-andy-griffith-show"`.

- `spinalCase("Teletubbies say Eh-oh")` should return `"teletubbies-say-eh-oh"`.

- `spinalCase("AllThe-small Things")` should return `"all-the-small-things"`.

---

## Solution

```js
function spinalCase(str) {
  // "It's such a fine line between stupid, and clever."
  // --David St. Hubbins
  str = str.replace(/([a-z])([A-Z])/g, '$1 $2');
  return str.replace(/\s+|_+/g, '-').toLowerCase();
}

spinalCase('This Is Spinal Tap');
```