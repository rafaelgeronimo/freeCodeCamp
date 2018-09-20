# Label Bootstrap Buttons

Just like we labeled our wells, we want to label our buttons.

Give each of your `button` elements text that corresponds to its `id`'s selector.

---

## Tips

- Give your `button` element with the id `target1` the text `#target1`.

- Give your `button` element with the id `target2` the text `#target2`.

- Give your `button` element with the id `target3` the text `#target3`.

- Give your `button` element with the id `target4` the text `#target4`.

- Give your `button` element with the id `target5` the text `#target5`.

- Give your `button` element with the id `target6` the text `#target6`.

---

## Solution

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```