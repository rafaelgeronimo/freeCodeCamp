# Understanding the Differences between the freeCodeCamp and Browser Console

You may have noticed that some freeCodeCamp JavaScript challenges include their own console. This console behaves a little differently than the browser console you used in the last challenge.

The following challenge is meant to highlight some of the differences between the freeCodeCamp console and the browser console.

First, the browser console. When you load and run an ordinary JavaScript file in your browser the `console.log()` statements will print exactly what you tell them to print to the browser console the exact number of times you requested. In your in-browser text editor the process is slightly different and can be confusing at first.

Values passed to `console.log()` in the text editor block run each set of tests as well as one more time for any function calls that you have in you code.

This lends itself to some interesting behavior and might trip you up in the beginning, because a logged value that you expect to see only once may print out many more times depending on the number of tests and the values being passed to those tests.

If you would like to see only your single output and not have to worry about running through the test cycles, you can use `console.clear()`.

---

## Challenge

Use `console.log()` to print the variables in the code where indicated.

---

## Tips

- Use `console.log()` to print the `outputTwo` variable. In your Browser Console this should print out the value of the variable two times.

- Use `console.log()` to print the `outputOne` variable.

- Use `console.clear()` to modify your output so that `outputOne` variable only outputs once.

---

## Solution

```js
// Open your browser console
let outputTwo = "This will print to the browser console 2 times";
// Use console.log() to print the outputTwo variable
console.log(outputTwo);

let outputOne = "Try to get this to log only once to the browser console";
// Use console.clear() in the next line to print the outputOne only once
console.clear();

// Use console.log() to print the outputOne variable
console.log(outputOne);
```