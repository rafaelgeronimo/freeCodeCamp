# Use Inheritance So You Don't Repeat Yourself

There's a principle in programming called `Don't Repeat Yourself (DRY)`. The reason repeated code is a problem is because any change requires fixing code in multiple places. This usually means more work for programmers and more room for errors.

Notice in the example below that the `describe` method is shared by `Bird` and `Dog`:

```js
Bird.prototype = {
  constructor: Bird,
  describe: function() {
    console.log("My name is " + this.name);
  }
};

Dog.prototype = {
  constructor: Dog,
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

The `describe` method is repeated in two places. The code can be edited to follow the `DRY` principle by creating a `supertype` (or parent) called `Animal`:

```js
function Animal() { };

Animal.prototype = {
  constructor: Animal,
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

Since `Animal` includes the `describe` method, you can remove it from `Bird` and `Dog`:

```js
Bird.prototype = {
  constructor: Bird
};

Dog.prototype = {
  constructor: Dog
};
```

---

## Challenge

The `eat` method is repeated in both `Cat` and `Bear`. Edit the code in the spirit of `DRY` by moving the eat method to the `Animal supertype`.

---

## Tips

- `Animal.prototype` should have the `eat` property.

- `Bear.prototype` should not have the `eat` property.

- `Cat.prototype` should not have the `eat` property.

---

## Solution

```js
function Cat(name) {
  this.name = name;
}

Cat.prototype = {
  constructor: Cat,
};

function Bear(name) {
  this.name = name;
}

Bear.prototype = {
  constructor: Bear,
};

function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};
```