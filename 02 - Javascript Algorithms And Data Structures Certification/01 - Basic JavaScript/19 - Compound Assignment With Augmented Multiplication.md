# Compound Assignment With Augmented Multiplication

The `*=` operator multiplies a variable by a number.

```js
myVar = myVar * 5;
```

will multiply `myVar` by `5`. This can be rewritten as:

```js
myVar *= 5;
```

---

## Challenge

Convert the assignments for `a`, `b`, and `c` to use the `*=` operator.

---

## Tips

- `a` should equal `25`

- `b` should equal `36`

- `c` should equal `46`

- You should use the `*=` operator for each variable

- Do not modify the code above the line

---

### Code before

```js
var a = 5;
var b = 12;
var c = 4.6;

// Only modify code below this line

a = a * 5;
b = 3 * b;
c = c * 10;

```

---

## Solution

```js
var a = 5;
var b = 12;
var c = 4.6;

// Only modify code below this line

a*= 5;
b*= 3;
c*= 10;

```