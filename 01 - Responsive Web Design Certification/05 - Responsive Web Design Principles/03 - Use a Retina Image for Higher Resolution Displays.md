# Use a Retina Image for Higher Resolution Displays

The simplest way to make your images appear "retina" (and optimize them for retina displays) is to define their `width` and `height` values as only half of what the original file is.

Here is an example of an image that is only using half of the original height and width:

```html
<style>
  img { height: 250px; width: 250px; }
</style>
<img src="coolPic500x500" alt="A most excellent picture">
```

---

## Challenge

Set the `width` and `height` of the `img` tag to half of their original values. In this case, both the original `height` and the original `width` are 200px.

---

## Tips

- Your `img` tag should have a `width` of 100 pixels.

- Your `img` tag should have a `height` of 100 pixels.

---

## Solution

```html
<style>
  img {
    width: 100px;
    height: 100px;
  }
</style>

<img src="https://s3.amazonaws.com/freecodecamp/FCCStickers-CamperBot200x200.jpg" alt="freeCodeCamp sticker that says 'Because CamperBot Cares'">
```