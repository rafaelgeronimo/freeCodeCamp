The next function of the `transform` property is `skewX()`, which skews the selected element along its X (horizontal) axis by a given degree.

The following code skews the paragraph element by -32 degrees along the X-axis.

```css
p {
  transform: skewX(-32deg);
}
```

---
**Challenge**

Skew the element with the id of `bottom` by 24 degrees along the X-axis by using the `transform` property.

---
**Tips**

- The element with id `bottom` should be skewed by 24 degrees along its X-axis.

---
**Solution**

```html
<style>
  div { 
    width: 70%;
    height: 100px;
    margin:  50px auto;
  }
  #top {
    background-color: red;
  }
  #bottom {
    background-color: blue;
    transform:skewX(24deg);
  }
</style>

<div id="top"></div>
<div id="bottom"></div>
```