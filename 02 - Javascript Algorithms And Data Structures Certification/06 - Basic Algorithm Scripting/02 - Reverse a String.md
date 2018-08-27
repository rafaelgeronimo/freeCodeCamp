# Reverse a String

Reverse the provided string.

You may need to turn the string into an array before you can reverse it.

Your result must be a string.

Remember to use [Read-Search-Ask](http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514) if you get stuck. Write your own code.

---

## Tips

- `reverseString("hello")` should return a string.

- `reverseString("hello")` should become `"olleh"`.

- `reverseString("Howdy")` should become `"ydwoH"`.

- `reverseString("Greetings from Earth")` should return `"htraE morf sgniteerG"`.

---

## Solution

```js
function reverseString(str) {
    let invert = [];
    for (let i = 0; i < str.length; i++){
      invert.unshift(str[i]);
    }
    return invert.join("");
}

reverseString("hello");
```