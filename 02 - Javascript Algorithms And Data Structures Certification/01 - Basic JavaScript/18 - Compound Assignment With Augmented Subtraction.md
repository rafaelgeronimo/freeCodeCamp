# Compound Assignment With Augmented Subtraction

Like the `+=` operator, `-=` subtracts a number from a variable.

```js
myVar = myVar - 5;
```

will subtract `5` from `myVar`. This can be rewritten as:

```js
myVar -= 5;
```

---

## Challenge

Convert the assignments for a, b, and c to use the -= operator.

## Tips

- `a` should equal `5`

-`b` should equal `-6`

- `c` should equal `2`

- You should use the `-=` operator for each variable

- Do not modify the code above the line

---

### Code before

```js
var a = 11;
var b = 9;
var c = 3;

// Only modify code below this line

a = a - 6;
b = b - 15;
c = c - 1;


```

---

## Solution

```js
var a = 11;
var b = 9;
var c = 3;

// Only modify code below this line

a-= 6;
b-= 15;
c-= 1;


```