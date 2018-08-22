# Find One or More Criminals in a Hunt

Time to pause and test your new regex writing skills. A group of criminals escaped from jail and ran away, but you don't know how many. However, you do know that they stay close together when they are around other people. You are responsible for finding all of the criminals at once.

Here's an example to review how to do this:

The regex `/z+/` matches the letter `z` when it appears one or more times in a row. It would find matches in all of the following strings:

```js
"z"
"zzzzzz"
"ABCzzzz"
"zzzzABC"
"abczzzzzzzzzzzzzzzzzzzzzabc"
```

But it does not find matches in the following strings since there are no letter `z` characters:

```js
""
"ABC"
"abcabc"
```

---

## Challenge

Write a `greedy` regex that finds one or more criminals within a group of other people. A criminal is represented by the capital letter `C`.

---

## Tips

- Your regex should match *one* criminal ("`C`") in `"C"`

- Your regex should match *two* criminals ("`CC`") in `"CC"`

- Your regex should match *three* criminals ("`CCC`") in `"P1P5P4CCCP2P6P3"`

- Your regex should match *five* criminals ("`CCCCC`") in `"P6P2P7P4P5CCCCCP3P1"`

- Your regex should not match any criminals in `""`

- Your regex should not match any criminals in `"P1P2P3"`

- Your regex should match *fifty* criminals ("`CCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCC`") in `"P2P1P5P4CCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCP3"`.

---

## Solution

```js
// example crowd gathering
let crowd = 'P1P2P3P4P5P6CCCP7P8P9';

let reCriminals = /C+/g; // Change this line

let matchedCriminals = crowd.match(reCriminals);
console.log(matchedCriminals);
```