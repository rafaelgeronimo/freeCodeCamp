# Split Your Bootstrap Row

Now that we have a Bootstrap Row, let's split it into two columns to house our elements.

Create two `div` elements within your row, both with the `class col-xs-6`.

---

## Tips

- Nest two `div class="col-xs-6"` elements within your `div class="row"` element.

- Make sure all your `div` elements have closing tags.

---

## Solution

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6"></div>
    <div class="col-xs-6"></div>
  </div>
</div>
```