# Pig Latin

Translate the provided string to pig latin.

Pig Latin takes the first consonant (or consonant cluster) of an English word, moves it to the end of the word and suffixes an "ay".

If a word begins with a vowel you just add "way" to the end.

Input strings are guaranteed to be English words in all lowercase.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `translatePigLatin("california")` should return "aliforniacay".

- `translatePigLatin("paragraphs")` should return "aragraphspay".

- `translatePigLatin("glove")` should return "oveglay".

- `translatePigLatin("algorithm")` should return "algorithmway".

- `translatePigLatin("eight")` should return "eightway".

- Should handle words where the first vowel comes in the end of the word.

- Should handle words without vowels.

---

## Solution

```js
function translatePigLatin(str) {
    let myRegex = /[aeiou]/gi;
     if(str.match(myRegex)){
        if(str[0].match(myRegex)){
            return str + "way";
        }
        else{
            let firstVoewl = str.indexOf(str.match(myRegex)[0]);
            return str.substr(firstVoewl) + str.substr(0, firstVoewl) + 'ay';
        }
     }else{
         return str + "ay";
     }
}

translatePigLatin("glove");
//translatePigLatin("algorithm");
```