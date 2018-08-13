# Appending Variables to Strings

Just as we can build a string over multiple lines out of string *literals*, we can also append variables to a string using the plus equals (`+=`) operator.

---

## Challenge

Set `someAdjective` and append it to `myStr` using the `+=` operator.

---

## Tips

- `someAdjective` should be set to a string at least 3 characters long

- Append `someAdjective` to `myStr` using the `+=` operator

---

### Code before

```js
    // Example
var anAdjective = "awesome!";
var ourStr = "freeCodeCamp is ";
ourStr += anAdjective;

// Only change code below this line

var someAdjective;
var myStr = "Learning to code is ";

```

---

## Solution

```js
    // Example
var anAdjective = "awesome!";
var ourStr = "freeCodeCamp is ";
ourStr += anAdjective;

// Only change code below this line

var someAdjective = "awesome";
var myStr = "Learning to code is ";

myStr += someAdjective;

```