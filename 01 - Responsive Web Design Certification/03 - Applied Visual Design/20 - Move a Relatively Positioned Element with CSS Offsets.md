The CSS offsets of `top` or `bottom`, and `left` or `right` tell the browser how far to offset an item relative to where it would sit in the normal flow of the document. You're offsetting an element away from a given spot, which moves the element away from the referenced side (effectively, the opposite direction). As you saw in the last challenge, using the top offset moved the h2 downwards. Likewise, using a left offset moves an item to the right.

![](https://i.imgur.com/eWWi3gZ.gif)

---
**Challenge**

Use CSS offsets to move the `h2` 15 pixels to the right and 10 pixels up.

---
**Tips**

- Your code should use a CSS offset to relatively position the `h2` 10px upwards. In other words, move it 10px away from the `bottom` of where it normally sits.

- Your code should use a CSS offset to relatively position the `h2` 15px towards the right. In other words, move it 15px away from the `left` of where it normally sits.

---
**Solution**

```html
<head>
<style>
  h2 {
    position: relative;
    bottom:10px;
    left:15px;
  }
</style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```