# Match Whitespace

The challenges so far have covered matching letters of the alphabet and numbers. You can also match the whitespace or spaces between letters.

You can search for whitespace using `\s`, which is a lowercase `s`. This pattern not only matches whitespace, but also carriage return, tab, form feed, and new line characters. You can think of it as similar to the character class `[ \r\t\f\n\v]`.

```js
let whiteSpace = "Whitespace. Whitespace everywhere!"
let spaceRegex = /\s/g;
whiteSpace.match(spaceRegex);
// Returns [" ", " "]
```

---

## Challenge

Change the regex `countWhiteSpace` to look for multiple whitespace characters in a string.

---

## Tips

- Your regex should use the global flag.

- Your regex should find eight spaces in `"Men are from Mars and women are from Venus."`

- Your regex should find three spaces in `"Space: the final frontier."`

- Your regex should find no spaces in `"MindYourPersonalSpace"`

---

## Solution

```js
let sample = "Whitespace is important in separating words";
let countWhiteSpace = /\s/g; // Change this line
let result = sample.match(countWhiteSpace);
```