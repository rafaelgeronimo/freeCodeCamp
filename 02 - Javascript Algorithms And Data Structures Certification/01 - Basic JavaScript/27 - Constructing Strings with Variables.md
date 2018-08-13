# Constructing Strings with Variables

Sometimes you will need to build a string, [Mad Libs](https://en.wikipedia.org/wiki/Mad_Libs) style. By using the concatenation operator (`+`), you can insert one or more variables into a string you're building.

---

## Challenge

Set `myName` to a string equal to your name and build `myStr` with `myName` between the strings `"My name is "` and `" and I am well!"`

---

## Tips

- `myName` should be set to a string at least 3 characters long

- Use two `+` operators to build `myStr` with `myName` inside it

---

### Code before

```js
// Example
var ourName = "freeCodeCamp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// Only change code below this line
var myName;
var myStr;

```

---

## Solution

```js
// Example
var ourName = "freeCodeCamp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// Only change code below this line
var myName = "Rafael";
var myStr = "My name is " + myName + " and I am well!";

```