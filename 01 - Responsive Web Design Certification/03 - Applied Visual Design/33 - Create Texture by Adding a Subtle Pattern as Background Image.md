One way to add texture and interest to a background and have it stand out more is to add a subtle pattern. The key is balance, as you don't want the background to stand out too much, and take away from the foreground. The `background` property supports the `url()` function in order to link to an image of the chosen texture or pattern. The link address is wrapped in quotes inside the parentheses.

---
**Challenge**

Using the url of `https://i.imgur.com/MJAkxbh.png`, set the `background` of the whole page with the `body` selector.

---
**Tips**

- Your `body` element should have a `background` property set to a `url()` with the given link.

---
**Solution**

```html
<style>
  body {
    background:url(https://i.imgur.com/MJAkxbh.png);
  }
</style>
```