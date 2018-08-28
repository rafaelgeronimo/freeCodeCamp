# Repeat a String Repeat a String

Repeat a given string `str` (first argument) for `num` times (second argument). Return an empty string if `num` is not a positive number.

Remember to use Read-Search-Ask if you get stuck. Write your own code.

---

## Tips

- `repeatStringNumTimes("*", 3)` should return `"***"`.

- `repeatStringNumTimes("abc", 3)` should return `"abcabcabc"`.

- `repeatStringNumTimes("abc", 4)` should return `"abcabcabcabc"`.

- `repeatStringNumTimes("abc", 1)` should return `"abc"`.

- `repeatStringNumTimes("*", 8)` should return `"********"`.

- `repeatStringNumTimes("abc", -2)` should return `""`.

- The built-in `repeat()` -method should not be used

---

```js
function repeatStringNumTimes(str, num) {
  // repeat after me
  if(num > 0){
      let temp = str;
      for(let i = 1; i < num; i++){
        console.log(i);
        str = str.concat(temp);
      }
  }else{
      str = "";
  }
  return str;
}

repeatStringNumTimes("abc", 3);
```