# Use Bracket Notation to Find the Nth Character in a String

You can also use *bracket notation* to get the character at other positions within a string.

Remember that computers start counting at `0`, so the first character is actually the zeroth character.

---

## Challenge

Let's try to set `thirdLetterOfLastName` to equal the third letter of the `lastName` variable using bracket notation.

**Hint**

Try looking at the `secondLetterOfFirstName` variable declaration if you get stuck.

---

## Tips

- The `thirdLetterOfLastName` variable should have the value of `v`.

- You should use bracket notation.

---

### Code before

```js
// Example
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var thirdLetterOfLastName = lastName;

```

---

## Solution

```js
// Example
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var thirdLetterOfLastName = lastName[2];

```