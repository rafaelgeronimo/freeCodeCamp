# Convert HTML Entities

Convert the characters `&`, `<`, `>`, `"` (double quote), and `'` (apostrophe), in a string to their corresponding HTML entities.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `convertHTML("Dolce & Gabbana")` should return `Dolce &​amp; Gabbana`.

- `convertHTML("Hamburgers < Pizza < Tacos")` should return `Hamburgers &​lt; Pizza &​lt; Tacos`.

- `convertHTML("Sixty > twelve")` should return `Sixty &​gt; twelve`.

- `convertHTML('Stuff in "quotation marks"')` should return `Stuff in &​quot;quotation marks&​quot;`.

- `convertHTML("Schindler's List")` should return `Schindler&​apos;s List`.

- `convertHTML("<>")` should return `&​lt;&​gt;`.

- `convertHTML("abc")` should return `abc`.

---

## Solution

```js
function convertHTML(str) {
  // &colon;&rpar;
   return str.replace(/&/g,"&​amp;").replace(/</g,"&​lt;").replace(/>/g,"&​gt;").replace(/\"/g,"&​quot;").replace(/\'/g,"&​apos;");
}

//convertHTML("Dolce & Gabbana");// should return Dolce &​amp; Gabbana.
//convertHTML("Hamburgers < Pizza < Tacos");// should return Hamburgers &​lt; Pizza &​lt; Tacos.
//convertHTML("Sixty > twelve");// should return Sixty &​gt; twelve.
//convertHTML('Stuff in "quotation marks"');// should return Stuff in &​quot;quotation marks&​quot;.
convertHTML("Schindler's List");// should return Schindler&​apos;s List.
//convertHTML("<>");// should return &​lt;&​gt;.
//convertHTML("abc");// should return abc.
```