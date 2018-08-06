The `repeating-linear-gradient()` function is very similar to ` linear-gradient()` with the major difference that it repeats the specified gradient pattern. `repeating-linear-gradient()` accepts a variety of values, but for simplicity, you'll work with an angle value and color stop values in this challenge.

The angle value is the direction of the gradient. Color stops are like width values that mark where a transition takes place, and are given with a percentage or a number of pixels.

In the example demonstrated in the code editor, the gradient starts with the color `yellow` at 0 pixels which blends into the second color `blue` at 40 pixels away from the start. Since the next color stop is also at 40 pixels, the gradient immediately changes to the third color `green`, which itself blends into the fourth color value `red` as that is 80 pixels away from the beginning of the gradient.

For this example, it helps to think about the color stops as pairs where every two colors blend together.

`0px [yellow -- blend -- blue] 40px [green -- blend -- red] 80px`

If every two color stop values are the same color, the blending isn't noticeable because it's between the same color, followed by a hard transition to the next color, so you end up with stripes.

---
**Challenge**

Make stripes by changing the `repeating-linear-gradient()` to use a gradient angle of `45deg`, then set the first two color stops to `yellow`, and finally the second two color stops to `black`.

---
**Tips**

- The angle of the `repeating-linear-gradient()` should be 45deg.

- The angle of the `repeating-linear-gradient()` should no longer be 90deg

- The color stop at 0 pixels should be `yellow`.

- One color stop at 40 pixels should be `yellow`.

- The second color stop at 40 pixels should be `black`.

- The last color stop at 80 pixels should be `black`.

---
**Solution**

```html
<style>

  div{ 
    border-radius: 20px;
    width: 70%;
    height: 400px;
    margin:  50 auto;
    background: repeating-linear-gradient(
      45deg,
      yellow 0px,
      yellow 40px,
      black 40px,
      black 80px
    );
  }

</style>

<div></div>
```