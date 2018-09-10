# Missing letters

Find the missing letter in the passed letter range and return it.

If all letters are present in the range, return undefined.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `fearNotLetter("abce")` should return "d".

- `fearNotLetter("abcdefghjklmno")` should return "i".

- `fearNotLetter("stvwx")` should return "u".

- `fearNotLetter("bcdf")` should return "e".

- `fearNotLetter("abcdefghijklmnopqrstuvwxyz")` should return undefined.

---

## Solution

```js
function fearNotLetter(str) {
    let letters = "abcdefghijklmnopqrstuvwxyz"
    let arr = [];
    for (let i in str){
        for(let j in letters){
            if (str[i] === letters[j]){
                arr.push(j);
            }
        }
    }
    for(let count in arr){
        if(arr[count] - (arr[count-1]) === 2){
            return(letters[arr[count]-1]);
        }
    }
}


fearNotLetter("abce");// should return "d".
//fearNotLetter("abcdefghjklmno");// should return "i".
//fearNotLetter("stvwx");// should return "u".
//fearNotLetter("bcdf");// should return "e".
//fearNotLetter("abcdefghijklmnopqrstuvwxyz");// should return undefined.
```