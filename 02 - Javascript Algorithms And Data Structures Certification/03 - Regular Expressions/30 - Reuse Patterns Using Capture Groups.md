# Reuse Patterns Using Capture Groups

Some patterns you search for will occur multiple times in a string. It is wasteful to manually repeat that regex. There is a better way to specify when you have multiple repeat substrings in your string.

You can search for repeat substrings using `capture groups`. Parentheses, `(` and `)`, are used to find repeat substrings. You put the regex of the pattern that will repeat in between the parentheses.

To specify where that repeat string will appear, you use a backslash (`\`) and then a number. This number starts at 1 and increases with each additional capture group you use. An example would be `\1` to match the first group.

The example below matches any word that occurs twice separated by a space:

```js
let repeatStr = "regex regex";
let repeatRegex = /(\w+)\s\1/;
repeatRegex.test(repeatStr); // Returns true
repeatStr.match(repeatRegex); // Returns ["regex regex", "regex"]
```

Using the `.match()` method on a string will return an array with the string it matches, along with its capture group.

---

## Challenge

Use `capture groups` in `reRegex` to match numbers that are repeated only three times in a string, each separated by a space.

---

## Tips

- Your regex should use the shorthand character class for digits.

- Your regex should reuse the capture group twice.

- Your regex should have two spaces separating the three numbers.

- Your regex should match `"42 42 42".`

- Your regex should match `"100 100 100".`

- Your regex should not match `"42 42 42 42".`

- Your regex should not match `"42 42".`

- Your regex should not match `"101 102 103".`

- Your regex should not match `"1 2 3".`

- Your regex should match `"10 10 10".`

---

## Solution

```js
let repeatNum = "42 42 42";
let reRegex = /^(\d+)\s\1\s\1$/; // Change this line
let result = reRegex.test(repeatNum);
```