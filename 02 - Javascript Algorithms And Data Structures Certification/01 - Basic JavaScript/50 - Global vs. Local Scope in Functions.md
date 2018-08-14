# Global vs. Local Scope in Functions

It is possible to have both *local* and *global* variables with the same name. When you do this, the `local` variable takes precedence over the `global` variable.

In this example:

```js
var someVar = "Hat";
function myFun() {
  var someVar = "Head";
  return someVar;
}
```

The function `myFun` will return `"Head"` because the `local` version of the variable is present.

---

## Challenge

Add a local variable to `myOutfit` function to override the value of `outerWear` with `"sweater"`.

---

## Tips

- Do not change the value of the global `outerWear`

- `myOutfit` should return `"sweater"`

- Do not change the return statement

---

### Code before

```js
// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line
  
  
  
  // Only change code above this line
  return outerWear;
}

myOutfit();
```

---

## Solution

```js
// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line
  var outerWear = "sweater";
   
  // Only change code above this line
  return outerWear;
}

myOutfit();
```