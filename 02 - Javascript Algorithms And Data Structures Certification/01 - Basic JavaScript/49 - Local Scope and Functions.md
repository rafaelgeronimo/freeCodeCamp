# Local Scope and Functions

Variables which are declared within a function, as well as the function parameters have *local* scope. That means, they are only visible within that function.

Here is a function `myTest` with a local variable called `loc`.

```js
function myTest() {
  var loc = "foo";
  console.log(loc);
}
myTest(); // logs "foo"
console.log(loc); // loc is not defined
```

loc is not defined outside of the function.

---

## Challenge

Declare a local variable `myVar` inside `myLocalScope`. Run the tests and then follow the instructions commented out in the editor.

### Hint

Refreshing the page may help if you get stuck.

---

## Tips

- No global `myVar` variable

- Add a local `myVar` variable

---

### Code before

```js
function myLocalScope() {
  'use strict'; // you shouldn't need to edit this line
  
  console.log(myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log(myVar);

// Now remove the console log line to pass the test
```

---

## Solution

```js
function myLocalScope() {
  'use strict'; // you shouldn't need to edit this line
  var myVar = 10;
  console.log(myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope


// Now remove the console log line to pass the test

```