# Use a span to Target Inline Elements

You can use spans to create inline elements. Remember when we used the btn-block class to make the button fill the entire row?

![Button Examples](https://i.imgur.com/PQTCbFp.png)

That illustrates the difference between an "inline" element and a "block" element.

By using the inline `span` element, you can put several elements on the same line, and even style different parts of the same line differently.

Nest the word "love" in your "Things cats love" element below within a `span` element. Then give that `span` the class `text-danger` to make the text red.

Here's how you would do this with the "Top 3 things cats hate" element:

```html
<p>Top 3 things cats <span class="text-danger">hate:</span></p>
```

---

## Tips

- Your `span` element should be inside your `p` element.

- Your `span` element should have just the text `love`.

- Your `span` element should have class `text-danger`.

- Make sure your `span` element has a closing tag.

---

## Solution

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>

  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <h2 class="text-primary text-center">CatPhotoApp</h2>

  <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```