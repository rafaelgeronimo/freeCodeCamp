# Arguments Optional

Create a function that sums two arguments together. If only one argument is provided, then return a function that expects one argument and returns the sum.

For example, `addTogether(2, 3)` should return `5`, and `addTogether(2)` should return a function.

Calling this returned function with a single argument will then return the sum:

```JS
var sumTwoAnd = addTogether(2);
```

`sumTwoAnd(3)` returns `5`.

If either argument isn't a valid number, return undefined.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `addTogether(2, 3)` should return 5.

- `addTogether(2)(3)` should return 5.

- `addTogether("http://bit.ly/IqT6zt")` should return undefined.

- `addTogether(2, "3")` should return undefined.

- `addTogether(2)([3])` should return undefined.

---

## Solution

```js
 function addTogether() {
      var checkNum = function(num) {
        if (typeof num !== 'number') {
          return undefined;
        } else
          return num;
      };
      if (arguments.length > 1) {
        var a = checkNum(arguments[0]);
        var b = checkNum(arguments[1]);
        if (a === undefined || b === undefined) {
          return undefined;
        } else {
          return a + b;
        }
      } else {
        var c = arguments[0];
        if (checkNum(c)) {
          return function(arg2) {
            if (c === undefined || checkNum(arg2) === undefined) {
              return undefined;
            } else {
              return c + arg2;
            }
          };
        }
      }
    }

//addTogether(2, 3);// should return 5.
addTogether(2)(3);// should return 5.
//addTogether("http://bit.ly/IqT6zt");// should return undefined.
//addTogether(2, "3");// should return undefined.
//addTogether(2)([3]);// should return undefined.
```