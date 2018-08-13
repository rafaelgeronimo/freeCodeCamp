# Concatenating Strings with Plus Operator

In JavaScript, when the `+` operator is used with a `String` value, it is called the *concatenation* operator. You can build a new string out of other strings by *concatenating* them together.

**Example**

`'My name is Alan,' + ' I concatenate.'`

**Note**

Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.

---

## Challenge

Build `myStr` from the strings `"This is the start. "` and `"This is the end."` using the `+` operator.

---

## Tips

- `myStr` should have a value of `This is the start. This is the end.`

- Use the `+` operator to build `myStr`

- `myStr` should be created using the `var` keyword.

- Make sure to assign the result to the `myStr` variable.

---

### Code before

```js
// Example
var ourStr = "I come first. " + "I come second.";

// Only change code below this line

var myStr;


```

## Solution

```js
// Example
var ourStr = "I come first. " + "I come second.";

// Only change code below this line

var myStr = "This is the start. " + "This is the end.";


```