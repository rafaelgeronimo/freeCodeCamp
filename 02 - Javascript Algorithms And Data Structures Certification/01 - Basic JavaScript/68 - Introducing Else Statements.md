# Introducing Else Statements

When a condition for an `if` statement is true, the block of code following it is executed. What about when that condition is false? Normally nothing would happen. With an `else` statement, an alternate block of code can be executed.

```js
if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}
```

---

## Challenge

Combine the `if` statements into a single `if/else` statement.

---

## Tips

- You should only have one `if` statement in the editor

- You should use an `else` statement

- `estElse(4)` should return "5 or Smaller"

- `estElse(5)` should return "5 or Smaller"

- `estElse(6)` should return "Bigger than 5"

- `testElse(10)` should return "Bigger than 5"

- Do not change the code above or below the lines.

---

### Code before

```js
function testElse(val) {
  var result = "";
  // Only change code below this line
  
  if (val > 5) {
    result = "Bigger than 5";
  }
  
  if (val <= 5) {
    result = "5 or Smaller";
  }
  
  // Only change code above this line
  return result;
}

// Change this value to test
testElse(4);
```

---

## Solution

```js
function testElse(val) {
  var result = "";
  if (val > 5) {
    result = "Bigger than 5";
  }else{
    result = "5 or Smaller";
  }
  return result;
}
testElse(4);
```