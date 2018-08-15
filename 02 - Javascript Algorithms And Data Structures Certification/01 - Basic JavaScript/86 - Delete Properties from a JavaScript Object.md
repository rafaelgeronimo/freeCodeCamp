# Delete Properties from a JavaScript Object

We can also delete properties from objects like this:

```js
delete ourDog.bark;
```

---

Delete the `"tails"` property from `myDog`. You may use either dot or bracket notation.

---

## Tips

- Delete the property `"tails"` from `myDog`.

- Do not modify the `myDog` setup

---

## Solution

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.
delete myDog["tails"];
```