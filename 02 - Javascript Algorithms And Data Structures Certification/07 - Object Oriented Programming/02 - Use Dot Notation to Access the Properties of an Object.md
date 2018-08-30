# Use Dot Notation to Access the Properties of an Object

The last challenge created an `object` with various `properties`, now you'll see how to access the values of those `properties`. Here's an example:

```js
let duck = {
  name: "Aflac",
  numLegs: 2
};
console.log(duck.name);
// This prints "Aflac" to the console
```

Dot notation is used on the `object` name, `duck`, followed by the name of the `property`, `name`, to access the value of "Aflac".

---

## Challenge

Print both `properties` of the `dog` object below to your console.

---

## Tips

- Your should use `console.log` to print the value for the `name` property of the `dog` object.

- Your should use `console.log` to print the value for the `numLegs` property of the `dog` object.

---

## Solution

```js
let dog = {
  name: "Spot",
  numLegs: 4
};
// Add your code below this line
console.log(dog.name);
console.log(dog.numLegs);
```