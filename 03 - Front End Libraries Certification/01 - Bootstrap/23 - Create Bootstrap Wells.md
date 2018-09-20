# Create Bootstrap Wells

Bootstrap has a class called `well` that can create a visual sense of depth for your columns.

Nest one `div` element with the class `well` within each of your `col-xs-6 div` elements.

---

## Tips

- Add a `div` element with the class `well` inside each of your `div` elements with the class `"col-xs-6"`

- Nest both of your `div` elements with the class `"col-xs-6"` within your `div` element with the class `"row"`.

- Make sure all your `div` elements have closing tags.

---

## Solution

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well"></div>
    </div>
    <div class="col-xs-6">
      <div class="well"></div>
    </div>
  </div>
</div>
```