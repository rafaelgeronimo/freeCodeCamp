# Match Beginning String Patterns

Prior challenges showed that regular expressions can be used to look for a number of matches. They are also used to search for patterns in specific positions in strings.

In an earlier challenge, you used the `caret` character (`^`) inside a `character set` to create a `negated character set` in the form `[^thingsThatWillNotBeMatched]`. Outside of a `character set`, the `caret` is used to search for patterns at the beginning of strings.

```js
let firstString = "Ricky is first and can be found.";
let firstRegex = /^Ricky/;
firstRegex.test(firstString);
// Returns true
let notFirst = "You can't find Ricky now.";
firstRegex.test(notFirst);
// Returns false
```

---

## Challenge

Use the `caret` character in a regex to find `"Cal"` only in the beginning of the string `rickyAndCal`.

---

## Tips

- Your regex should search for `"Cal"` with a capital letter.

- Your regex should not use any flags.

- Your regex should match `"Cal"` at the beginning of the string.

- Your regex should not match `"Cal"` in the middle of a string.

---

## Solution

```js

```