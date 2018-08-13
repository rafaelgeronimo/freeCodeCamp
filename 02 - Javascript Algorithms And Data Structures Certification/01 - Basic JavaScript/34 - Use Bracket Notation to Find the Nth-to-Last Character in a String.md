# Use Bracket Notation to Find the Nth-to-Last Character in a String

You can use the same principle we just used to retrieve the last character in a string to retrieve the Nth-to-last character.

For example, you can get the value of the third-to-last letter of the `var firstName = "Charles"` string by using `firstName[firstName.length - 3]`

---

## Challenge

Use *bracket notation* to find the second-to-last character in the `lastName` string.

**Hint**

Try looking at the `thirdToLastLetterOfFirstName` variable declaration if you get stuck.

---

## Tips

- `secondToLastLetterOfLastName` should be "c".

- You have to use `.length` to get the second last letter.

---

### Code before

```js
// Example
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// Setup
var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName;
```

---

## Solution

```js
// Example
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// Setup
var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName[lastName.length -2];
```