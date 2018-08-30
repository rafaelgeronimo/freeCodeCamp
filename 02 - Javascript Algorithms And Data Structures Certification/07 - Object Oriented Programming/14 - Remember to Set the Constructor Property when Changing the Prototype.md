# Remember to Set the Constructor Property when Changing the Prototype

There is one crucial side effect of manually setting the `prototype` to a new object. It erased the `constructor` property! The code in the previous challenge would print the following for `duck`:

```js
console.log(duck.constructor)
// prints ‘undefined’ - Oops!
```

To fix this, whenever a prototype is manually set to a new object, remember to define the `constructor` property:

```js
Bird.prototype = {
  constructor: Bird, // define the constructor property
  numLegs: 2,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

---

## Challenge

Define the `constructor` property on the `Dog prototype`.

---

## Tips

- `Dog.prototype` should set the `constructor` property.

---

## Solution

```js
function Dog(name) {
  this.name = name;
}

// Modify the code below this line
Dog.prototype = {
  constructor: Dog,
  numLegs: 2,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```