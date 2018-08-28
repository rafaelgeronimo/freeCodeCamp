# Title Case a Sentence

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".

Remember to use Read-Search-Ask if you get stuck. Write your own code.

---

## Tips

- `titleCase("I'm a little tea pot")` should return a string.

- `titleCase("I'm a little tea pot")` should return `I'm A Little Tea Pot`.

- `titleCase("sHoRt AnD sToUt")` should return `Short And Stout`.

- `titleCase("HERE IS MY HANDLE HERE IS MY SPOUT")` should return `Here Is My Handle Here Is My Spout`.

---

## Solution

```js
function titleCase(str) {
    let arr = [...str];
    for (let i in arr){
        arr[0] = arr[0].toUpperCase();
        if ((arr[i-1]) === " "){
            arr[i] = arr[i].toUpperCase();
        }else{
            arr[i] = arr[i].toLowerCase();
        }
    }
    return arr.join("");
}

//titleCase("I'm a little tea pot");// should return I'm A Little Tea Pot.
//titleCase("sHoRt AnD sToUt");// should return Short And Stout.
titleCase("HERE IS MY HANDLE HERE IS MY SPOUT");// should return Here Is My Handle Here Is My Spout.
```