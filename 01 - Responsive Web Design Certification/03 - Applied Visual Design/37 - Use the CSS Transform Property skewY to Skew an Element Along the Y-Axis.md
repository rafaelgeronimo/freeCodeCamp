Given that the `skewX()` function skews the selected element along the X-axis by a given degree, it is no surprise that the `skewY()` property skews an element along the Y (vertical) axis.

---
**Challenge**

Skew the element with the id of `top` -10 degrees along the Y-axis by using the `transform` property.

---
**Tips**

- The element with id `top` should be skewed by -10 degrees along its Y-axis.

---
**Solution**

```html
<style>
  div { 
    width: 70%;
    height: 100px;
    margin: 50px auto;
  }
  #top {
    background-color: red;
    transform:skewY(-10deg);
  }
  #bottom {
    background-color: blue;
    transform: skewX(24deg);
  }
</style>

<div id="top"></div>
<div id="bottom"></div>
```