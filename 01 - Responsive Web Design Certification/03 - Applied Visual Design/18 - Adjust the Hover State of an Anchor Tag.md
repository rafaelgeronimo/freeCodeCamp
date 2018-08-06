This challenge will touch on the usage of pseudo-classes. A pseudo-class is a keyword that can be added to selectors, in order to select a specific state of the element.

For example, the styling of an anchor tag can be changed for its hover state using the `:hover` pseudo-class selector. Here's the CSS to change the `color` of the anchor tag to red during its hover state:

```css
a:hover {
  color: red;
}
```

---
**Challenge**

The code editor has a CSS rule to style all `a` tags black. Add a rule so that when the user hovers over the `a` tag, the `color` is blue.

---
**Tips**:

- The anchor tag `color` should remain black, only add CSS rules for the `:hover` state.

- The anchor tag should have a `color` of blue on hover.

---
**Solution**:
```html
<style>
  a {
    color: #000;
  }
  a:hover{
    color:blue;
  }
</style>
<a href="http://freecatphotoapp.com/" target="_blank">CatPhotoApp</a>
```