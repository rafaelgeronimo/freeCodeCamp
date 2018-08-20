# Use Destructuring Assignment to Pass an Object as a Function's Parameters

In some cases, you can destructure the object in a function argument itself.

Consider the code below:

```js
const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;
  // do something with these variables
}
```

This effectively destructures the object sent into the function. This can also be done in-place:

```js
const profileUpdate = ({ name, age, nationality, location }) => {
  /* do something with these fields */
}
```

This removes some extra lines and makes our code look neat.

This has the added benefit of not having to manipulate an entire object in a function; only the fields that are needed are copied inside the function.

---

## Challenge

Use destructuring assignment within the argument to the function `half` to send only `max` and `min` inside the function.

---

## Tips

- `stats` should be an `object`.

- `half(stats)` should be `28.015`

- Destructuring was used.

---

## Solution

```js

```