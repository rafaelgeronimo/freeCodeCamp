# Use @for to Create a Sass Loop

The `@for` directive adds styles in a loop, very similar to a `for` loop in JavaScript.

`@for` is used in two ways: "start through end" or "start to end". The main difference is that "start to end" *excludes* the end number, and "start through end" *includes* the end number.

Here's a start **through** end example:

```scss
@for $i from 1 through 12 {
  .col-#{$i} { width: 100%/12 * $i; }
}
```

The `#{$i}` part is the syntax to combine a variable (`i`) with text to make a string. When the Sass file is converted to CSS, it looks like this:

```css
.col-1 {
  width: 8.33333%;
}

.col-2 {
  width: 16.66667%;
}

...

.col-12 {
  width: 100%;
}
```

This is a powerful way to create a grid layout. Now you have twelve options for column widths available as CSS classes.

---

## Challenge

Write a `@for` directive that takes a variable `$j` that goes from 1 **to** 6.

It should create 5 classes called `.text-1` to `.text-5` where each has a `font-size` set to 10px multiplied by the index.

---

## Tips

- Your code should use the `@for` directive.

- Your `.text-1` class should have a `font-size` of 10px.

- Your `.text-2` class should have a `font-size` of 20px.

- Your `.text-3` class should have a `font-size` of 30px.

- Your `.text-4` class should have a `font-size` of 40px.

- Your `.text-5` class should have a `font-size` of 50px.

---

## Solution

```html
<style type='text/sass'>
  @for $i from 1 to 6 {
    .text-#{$i} { font-size: 10 * $i; }
  }  
</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
```