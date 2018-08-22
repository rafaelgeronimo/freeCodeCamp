# Match Non-Whitespace Characters

You learned about searching for whitespace using `\s`, with a lowercase `s`. You can also search for everything except whitespace.

Search for non-whitespace using `\S`, which is an uppercase `s`. This pattern will not match whitespace, carriage return, tab, form feed, and new line characters. You can think of it being similar to the character class `[^ \r\t\f\n\v]`.

```js
let whiteSpace = "Whitespace. Whitespace everywhere!"
let nonSpaceRegex = /\S/g;
whiteSpace.match(nonSpaceRegex).length; // Returns 32
```

---

## Challenge

Change the regex `countNonWhiteSpace` to look for multiple non-whitespace characters in a string.

---

## Tips

- Your regex should use the global flag.

- Your regex should find 35 non-spaces in `"Men are from Mars and women are from Venus."`

- Your regex should find 23 non-spaces in `"Space: the final frontier."`

- Your regex should find 21 non-spaces in `"MindYourPersonalSpace"`

---

## Solution

```js
let sample = "Whitespace is important in separating words";
let countNonWhiteSpace = /\S/g; // Change this line
let result = sample.match(countNonWhiteSpace);
```