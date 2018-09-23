# Apply a Style Until a Condition is Met with @while

The `@while` directive is an option with similar functionality to the JavaScript `while` loop. It creates CSS rules until a condition is met.

The `@for` challenge gave an example to create a simple grid system. This can also work with `@while`.

```scss
$x: 1;
@while $x < 13 {
  .col-#{$x} { width: 100%/12 * $x;}
  $x: $x + 1;
}
```

First, define a variable `$x` and set it to 1. Next, use the `@while` directive to create the grid system *while* `$x` is less than 13.

After setting the CSS rule for `width`, `$x` is incremented by 1 to avoid an infinite loop.

---

## Challenge

Use `@while` to create a series of classes with different `font-sizes`.

There should be 10 different classes from `text-1` to `text-10`. Then set `font-size` to 5px multiplied by the current index number. Make sure to avoid an infinite loop!

---

## Tips

- Your code should use the `@while` directive.

- Your code should set an index variable to 1 to start.

- Your code should increment the counter variable.

- Your `.text-1` class should have a `font-size` of 5px.

- Your `.text-2` class should have a `font-size` of 10px.

- Your `.text-3` class should have a `font-size` of 15px.

- Your `.text-4` class should have a `font-size` of 20px.

- Your `.text-5` class should have a `font-size` of 25px.

- Your `.text-6` class should have a `font-size` of 30px.

- Your `.text-7` class should have a `font-size` of 35px.

- Your `.text-8` class should have a `font-size` of 40px.

- Your `.text-9` class should have a `font-size` of 45px.

- Your `.text-10` class should have a `font-size` of 50px.

---

## Solution

```html
<style type='text/sass'>
  $x: 1;
@while $x < 11 {
    .text-#{$x} { font-size: 5 * $x};
    $x: $x + 1;
}  
</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
<p class="text-6">Hello</p>
<p class="text-7">Hello</p>
<p class="text-8">Hello</p>
<p class="text-9">Hello</p>
<p class="text-10">Hello</p>
```