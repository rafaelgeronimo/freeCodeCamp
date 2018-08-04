HTML has a special element for creating `unordered lists`, or bullet point style lists.

Unordered lists start with an opening `<ul>` element, followed by any number of `<li>` elements. Finally, unordered lists close with a `</ul>`

For example:

```
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

would create a bullet point style list of "milk" and "cheese".

---
Remove the last two `p` elements and create an unordered list of three things that cats love at the bottom of the page.

---
**Resolução**:
```
<h2>CatPhotoApp</h2>
<main>
  <p>Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
<ul>
  <li>Comer</li>
  <li>Dormir</li>
  <li>Brincar</li>
</ul>
```