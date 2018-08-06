The next layout scheme that CSS offers is the `fixed` position, which is a type of absolute positioning that locks an element relative to the browser window. Similar to absolute positioning, it's used with the CSS offset properties and also removes the element from the normal flow of the document. Other items no longer "realize" where it is positioned, which may require some layout adjustments elsewhere.

One key difference from the `absolute` position is that the element won't move when the user scrolls.

---
**Challenge**
The navigation bar in the code is labeled with an id of `navbar`. Change its `position` to `fixed`, and offset it 0 pixels from the `top` and 0 pixels from the `left`. Notice the (lack of) impact to the `h1` position, it hasn't been pushed down to accommodate the navigation bar and would need to be adjusted separately.

---
**Tips**

- The `#navbar` element should have a `position` set to `fixed`.

- Your code should use the `top` CSS offset of 0 pixels on the `#navbar` element.

- Your code should use the `left` CSS offset of 0 pixels on the `#navbar` element.

---
**Solution**
```html
<style>
  #navbar {
    position:fixed;
    top: 0px;
    left: 0px;
    width: 100%;
    background-color: #767676;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
  }
</style>
<body>
  <header>
    <h1>Welcome!</h1>
    <nav id="navbar">
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Contact</a></li>
      </ul>
    </nav>
  </header>
  <p>I shift up when the #navbar is fixed to the browser window.</p>
</body>
```