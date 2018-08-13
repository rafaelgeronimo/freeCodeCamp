# Escape Sequences in Strings

Quotes are not the only characters that can be *escaped* inside a string. There are two reasons to use escaping characters: First is to allow you to use characters you might not otherwise be able to type out, such as a backspace. Second is to allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean. We learned this in the previous challenge.

|**Code**|**Output**|
|---|---|
|\'|single quote|
|\"|double quote|
|\\|backslash|
|\n|newline|
|\r|carriage return|
|\t|tab|
|\b|backspace|
|\f|form feed|

*Note that the backslash itself must be escaped in order to display as a backslash.*

---

## Challenge

Assign the following three lines of text into the single variable `myStr` using escape sequences.

```
FirstLine
    \SecondLine
ThirdLine
```

You will need to use escape sequences to insert special characters correctly. You will also need to follow the spacing as it looks above, with no spaces between escape sequences or words.

Here is the text with the escape sequences written out.

"FirstLine `newlinetabbackslash` SecondLine `newline` ThirdLine"

---

## Tips

- `myStr` should not contain any spaces

- `myStr` should contain the strings `FirstLine`, `SecondLine` and `ThirdLine` (remember case sensitivity)

- `FirstLine` should be followed by the newline character `\n`

- `myStr` should contain a tab character `\t` which follows a newline character

- `SecondLine` should be preceded by the backslash character `\\`

- There should be a newline character between `SecondLine` and `ThirdLine`

---

### Code before

```js
var myStr; // Change this line

```

---

## Solution

```js
var myStr = "FirstLine\n\tSecondLine\nThirdLine";

```