# Split a String into an Array Using the split Method

The `split` method splits a string into an array of strings. It takes an argument for the delimiter, which can be a character to use to break up the string or a regular expression. For example, if the delimiter is a space, you get an array of words, and if the delimiter is an empty string, you get an array of each character in the string.

Here are two examples that split one string by spaces, then another by digits using a regular expression:

```js
var str = "Hello World";
var bySpace = str.split(" ");
// Sets bySpace to ["Hello", "World"]

var otherString = "How9are7you2today";
var byDigits = otherString.split(/\d/);
// Sets byDigits to ["How", "are", "you", "today"]
```

Since strings are immutable, the `split` method makes it easier to work with them.

---

## Challenge

Use the `split` method inside the `splitify` function to split `str` into an array of words. The function should return the array. Note that the words are not always separated by spaces, and the array should not contain punctuation.

---

## Tips

- Your code should use the `split` method.

 `splitify("Hello World,I-am code")` should return `["Hello", "World", "I", "am", "code"]`.

- `splitify("Earth-is-our home")` should return `["Earth", "is", "our", "home"]`.

- `splitify("This.is.a-sentence")` should return `["This", "is", "a", "sentence"]`.

---

## Solution

```js
function splitify(str) {
  // Add your code below this line
  var arr = str.split(/\W/g);
  return arr;  
  // Add your code above this line
}
splitify("Hello World,I-am code");
```