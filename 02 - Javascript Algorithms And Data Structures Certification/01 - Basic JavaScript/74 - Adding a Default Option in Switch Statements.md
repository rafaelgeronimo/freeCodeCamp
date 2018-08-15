# Adding a Default Option in Switch Statements

In a `switch` statement you may not be able to specify all possible values as `case` statements. Instead, you can add the `default` statement which will be executed if no matching `case` statements are found. Think of it like the final `else` statement in an `if/else` chain.

A `default` statement should be the last case.

```js
switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}
```

## Challenge

Write a switch statement to set `answer` for the following conditions:
`"a"` - "apple"
`"b"` - "bird"
`"c"` - "cat"
`default` - "stuff"

---

## Tips

- `switchOfStuff("a")` should have a value of "apple"

- `switchOfStuff("b")` should have a value of "bird"

- `switchOfStuff("c")` should have a value of "cat"

- `switchOfStuff("d")` should have a value of "stuff"

- `switchOfStuff(4)` should have a value of "stuff"

- You should not use any `if` or `else` statements

- You should use a `default` statement

- You should have at least 3 `break` statements

---

## Solution

```js
function switchOfStuff(val) {
  var answer = "";
  switch(val) {
    case "a":
      return "apple";
      break;
    case "b":
      return "bird";
      break;
    case "c":
      return "cat";
      break;
    default:
      return "stuff";
      break;
  }
  return answer;  
}
switchOfStuff(1);

```