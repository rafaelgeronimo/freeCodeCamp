# Understanding Undefined Value returned from a Function

A function can include the `return` statement but it does not have to. In the case that the function doesn't have a `return` statement, when you call it, the function processes the inner code but the returned value is `undefined`.

## Example

```js
var sum = 0;
function addSum(num) {
  sum = sum + num;
}
var returnedValue = addSum(3); // sum will be modified but returned value is undefined
```

`addSum` is a function without a `return` statement. The function will change the global `sum` variable but the returned value of the function is `undefined`

---

## Challenge

Create a function `addFive` without any arguments. This function adds 5 to the `sum` variable, but its returned value is `undefined`.

---

## Tips

- `addFive` should be a function

- `sum` should be equal to 8

- Returned value from `addFive` should be `undefined`

- Inside of your functions, add 5 to the `sum` variable

---

### Code before

```js
// Example
var sum = 0;
function addThree() {
  sum = sum + 3;
}

// Only change code below this line



// Only change code above this line
var returnedValue = addFive();
```

---

## Solution

```js
// Example
var sum = 0;
function addThree() {
  sum = sum + 3;
}

// Only change code below this line
function addFive(){
  sum += 5;
}

// Only change code above this line
var returnedValue = addFive();
```