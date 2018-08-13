# Concatenating Strings with the Plus Equals Operator

We can also use the `+=` operator to *concatenate* a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.

**Note**

Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.

---

## Challenge

Build `myStr` over several lines by concatenating these two strings: `"This is the first sentence. "` and `"This is the second sentence."` using the `+=` operator. Use the `+=` operator similar to how it is shown in the editor. Start by assigning the first string to `myStr`, then add on the second string.

---

## Tips

- `myStr` should have a value of `This is the first sentence. This is the second sentence.`

- Use the `+=` operator to build myStr

---

### Code before

```js
// Example
var ourStr = "I come first. ";
ourStr += "I come second.";

// Only change code below this line

var myStr;


```

---

## Solution

```js
// Example
var ourStr = "I come first. ";
ourStr += "I come second.";

// Only change code below this line

var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";

```