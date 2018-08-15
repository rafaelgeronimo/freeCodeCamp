# Add New Properties to a JavaScript Object

You can add new properties to existing JavaScript objects the same way you would modify them.

Here's how we would add a `"bark"` property to `ourDog`:

```js
ourDog.bark = "bow-wow";
```

or

```js
ourDog["bark"] = "bow-wow";
```

Now when we evaluate `ourDog.bark`, we'll get his bark, "bow-wow".

---

## Challenge

Add a `"bark"` property to `myDog` and set it to a dog sound, such as "woof". You may use either dot or bracket notation.

---

## Tips

- Add the property `"bark"` to `myDog`.

- Do not add `"bark"` to the setup section

---

## Solution

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.bark = "bow-wow";

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.
myDog["bark"] = "woof";
```