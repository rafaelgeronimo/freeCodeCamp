# Use an Array to Store a Collection of Data

The below is an example of the simplest implementation of an array data structure. This is known as a *one-dimensional array*, meaning it only has one level, or that it does not have any other arrays nested within it. Notice it contains *booleans*, *strings*, and *numbers*, among other valid JavaScript data types:

```js
let simpleArray = ['one', 2, 'three’, true, false, undefined, null];
console.log(simpleArray.length);
// logs 7
```

All array's have a length property, which as shown above, can be very easily accessed with the syntax `Array.length`.

A more complex implementation of an array can be seen below. This is known as a *multi-dimensional array*, or an array that contains other arrays. Notice that this array also contains JavaScript *objects*, which we will examine very closely in our next section, but for now, all you need to know is that arrays are also capable of storing complex objects.

```js
let complexArray = [
  [
    {
      one: 1,
      two: 2
    },
    {
      three: 3,
      four: 4
    }
  ],
  [
    {
      a: "a",
      b: "b"
    },
    {
      c: "c",
      d: “d”
    }
  ]
];
```

---

## Challenge

We have defined a variable called `yourArray`. Complete the statement by assigning an array of at least 5 elements in length to the `yourArray` variable. Your array should contain at least one *string*, one *number*, and one *boolean*.

---

## Tips

- yourArray is an array

- `yourArray` is at least 5 elements long

- `yourArray` contains at least one `boolean`

- `yourArray` contains at least one `number`

- `yourArray` contains at least one `string`

---

## Solution

```js
let yourArray = [1, "Hello", true, 2, "World"]; // change this line
```