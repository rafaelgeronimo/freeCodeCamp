# Return a Value from a Function with Return

We can pass values into a function with *arguments*. You can use a `return` statement to send a value back out of a function.

## Example

```js
function plusThree(num) {
  return num + 3;
}
var answer = plusThree(5); // 8
```

`plusThree` takes an *argument* for `num` and returns a value equal to `num + 3`.

---

## Challenge

Create a function `timesFive` that accepts one argument, multiplies it by `5`, and returns the new value. See the last line in the editor for an example of how you can test your `timesFive` function.

---

## Tips

- `timesFive` should be a function

- `timesFive(5)` should return `25`

- `timesFive(2)` should return `10`

- `timesFive(0)` should return `0`

---

### Code before

```js
// Example
function minusSeven(num) {
  return num - 7;
}

// Only change code below this line



console.log(minusSeven(10));
```

---

## Solution

```js
// Example
function minusSeven(num) {
  return num - 7;
}

// Only change code below this line
function timesFive(num){
  return num * 5;
}

console.log(minusSeven(10));
```