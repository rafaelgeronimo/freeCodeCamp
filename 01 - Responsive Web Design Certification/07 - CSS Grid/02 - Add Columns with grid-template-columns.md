# Add Columns with grid-template-columns

Simply creating a grid element doesn't get you very far. You need to define the structure of the grid as well. To add some columns to the grid, use the `grid-template-columns` property on a grid container as demonstrated below:

```css
.container {
  display: grid;
  grid-template-columns: 50px 50px;
}
```

This will give your grid two columns that are 50px wide each.

The number of parameters given to the `grid-template-columns` property indicates the number of columns in the grid, and the value of each parameter indicates the width of each column.

---

## Challenge

Give the grid container three columns that are `100px` wide each.

---

## Tips

- `container` class should have a `grid-template-columns` property with three units of `100px`.

---

## Solution

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* add your code below this line */
    grid-template-columns: 100px 100px 100px;

    /* add your code above this line */
  }
</style>
  
<div class="container">
  <div class="d1">1</div>
  <div class="d2">2</div>
  <div class="d3">3</div>
  <div class="d4">4</div>
  <div class="d5">5</div>
</div>
```