# Factorialize a Number

Return the factorial of the provided integer.

If the integer is represented with the letter n, a factorial is the product of all positive integers less than or equal to n.

Factorials are often represented with the shorthand notation `n!`

For example: `5! = 1 * 2 * 3 * 4 * 5 = 120`

Only integers greater than or equal to zero will be supplied to the function.

Remember to use [Read-Search-Ask](http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514) if you get stuck. Write your own code.

---

## Tips

- `factorialize(5)` should return a number.

- `factorialize(5)` should return 120.

- `factorialize(10)` should return 3628800.

- `factorialize(20)` should return 2432902008176640000.

- `factorialize(0)` should return 1.

---

## Solution

```js
function factorialize(num) {
    let result = 1;
    for (let i = 1; i <= num; i++){
        result = result * i;
    }
    return result;
}

factorialize(5);
```