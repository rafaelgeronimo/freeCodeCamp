# Use the flex-basis Property to Set the Initial Size of an Item

The `flex-basis` property specifies the initial size of the item before CSS makes adjustments with `flex-shrink` or `flex-grow`.

The units used by the `flex-basis` property are the same as other size properties (`px`, `em`, `%`, etc.). The value `auto` sizes items based on the content.

---

## Challenge

Set the initial size of the boxes using `flex-basis`. Add the CSS property `flex-basis` to both `#box-1` and `#box-2`. Give `#box-1` a value of `10em` and `#box-2` a value of `20em`.

---

## Tips

- The `#box-1` element should have a `flex-basis` property.

- The `#box-1` element should have a `flex-basis` value of `10em`.

- The `#box-2` element should have the `flex-basis` property.

- The `#box-2` element should have a `flex-basis` value of `20em`.

---

## Solution

```html
<style>
  #box-container {
    display: flex;
    height: 500px;
  }
  
  #box-1 {
    background-color: dodgerblue;
    height: 200px;
    flex-basis:10em;
  }
  
  #box-2 {
    background-color: orangered;
    height: 200px;
    flex-basis:20em;
  }
</style>
  
<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>
```