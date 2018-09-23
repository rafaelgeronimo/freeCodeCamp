# Use @if and @else to Add Logic To Your Styles

The `@if` directive in Sass is useful to test for a specific case - it works just like the `if` statement in JavaScript.

```scss
@mixin make-bold($bool) {
  @if $bool == true {
    font-weight: bold;
  }
}
```

And just like in JavaScript, `@else if` and `@else` test for more conditions:

```scss
@mixin text-effect($val) {
  @if $val == danger {
    color: red;
  }
  @else if $val == alert {
    color: yellow;
  }
  @else if $val == success {
    color: green;
  }
  @else {
    color: black;
  }
}
```

---

## Challenge

Create a `mixin` called `border-stroke` that takes a parameter `$val`. The `mixin` should check for the following conditions using `@if`, `@else if`, and `@else`:

```css
light - 1px solid black
medium - 3px solid black
heavy - 6px solid black
none - no border
```

---

## Tips

- Your code should declare a `mixin` named `border-stroke` which has a parameter named `$val`.

- Your `mixin` should have an `@if` statement to check if `$val` is light, and to set the `border` to 1px solid black.

- Your mixin should have an `@else if` statement to check if `$val` is medium, and to set the border to 3px solid black.

- Your `mixin` should have an `@else if` statement to check if `$val` is heavy, and to set the border to 6px solid black.

- Your `mixin` should have an `@else` statement to set the `border` to none.

---

## Solution

```html
<style type='text/sass'>
  @mixin border-stroke($val) {
    @if $val == light {
      border: 1px solid black;
    }
    @else if $val == medium {
      border: 3px solid black;
    }
    @else if $val == heavy {
      border: 6px solid black;
    }
    @else {
      border: none;
    }
  }
  
  
  #box {
    width: 150px;
    height: 150px;
    background-color: red;
    @include border-stroke(medium);
  }  
</style>

<div id="box"></div>
```