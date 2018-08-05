Now we've proven that every HTML page has a `body` element, and that its `body` element can also be styled with CSS.

Remember, you can style your `body` element just like any other HTML element, and all your other elements will inherit your `body` element's styles.

---
First, create a `h1` element with the text `Hello World`

Then, let's give all elements on your page the color of `green` by adding `color: green;` to your `body` element's style declaration.

Finally, give your `body` element the font-family of `monospace` by adding `font-family: monospace;` to your `body` element's style declaration.

---
**Tips**:
- Create an h1 element.

- Your h1 element should have the text Hello World.

- Make sure your h1 element has a closing tag.

- Give your body element the color property of green.

- Give your body element the font-family property of monospace.

- Your h1 element should inherit the font monospace from your body element.

- Your h1 element should inherit the color green from your body element.

---
**Resolution**:
```
<style>
  body {
    background-color: black;
    color: green;
    font-family: monospace;
  }

</style>
<h1>Hello World</h1>
```