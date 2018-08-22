# Match All Numbers

You've learned shortcuts for common string patterns like alphanumerics. Another common pattern is looking for just digits or numbers.

The shortcut to look for digit characters is `\d`, with a lowercase `d`. This is equal to the character class `[0-9]`, which looks for a single character of any number between zero and nine.

---

## Challenge

Use the shorthand character class `\d` to count how many digits are in movie titles. Written out numbers ("six" instead of 6) do not count.

---

## Tips

- Your regex should use the shortcut character to match digit characters

- Your regex should use the global flag.

- Your regex should find 1 digit in `"9"`.

- Your regex should find 2 digits in `"Catch 22"`.

- Your regex should find 3 digits in `"101 Dalmatians"`.

- Your regex should find no digits in `"One, Two, Three"`.

- Your regex should find 2 digits in `"21 Jump Street"`.

- Your regex should find 4 digits in `"2001: A Space Odyssey"`.

---

## Solution

```js
let numString = "Your sandwich will be $5.00";
let numRegex = /\d/g; // Change this line
let result = numString.match(numRegex).length;
```