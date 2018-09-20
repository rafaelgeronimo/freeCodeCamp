# Give Each Element a Unique id

We will also want to be able to use jQuery to target each button by its unique id.

Give each of your buttons a unique id, starting with `target1` and ending with `target6`.

Make sure that `target1` to `target3` are in `#left-well`, and `target4` to `target6` are in `#right-well`.

---

## Tips

- One `button` element should have the id `target1`.

- One `button` element should have the id `target2`.

- One `button` element should have the id `target3`.

- One `button` element should have the id `target4`.

- One `button` element should have the id `target5`.

- One `button` element should have the id `target6`.

---

## Solution

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1"></button>
        <button class="btn btn-default target" id="target2"></button>
        <button class="btn btn-default target" id="target3"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4"></button>
        <button class="btn btn-default target" id="target5"></button>
        <button class="btn btn-default target" id="target6"></button>
      </div>
    </div>
  </div>
</div>
```