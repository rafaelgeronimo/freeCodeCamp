# Create a Complex JSX Element

The last challenge was a simple example of JSX, but JSX can represent more complex HTML as well.

One important thing to know about nested JSX is that it must return a single element.

This one parent element would wrap all of the other levels of nested elements.

For instance, several JSX elements written as siblings with no parent wrapper element will not transpile.

Here's an example:

**Valid JSX:**

```html
<div>
  <p>Paragraph One</p>
  <p>Paragraph Two</p>
  <p>Paragraph Three</p>
</div>
```

**Invalid JSX:**

```html
<p>Paragraph One</p>
<p>Paragraph Two</p>
<p>Paragraph Three</p>
```

---

## Challenge

Define a new constant `JSX` that renders a `div` which contains the following elements in order:

An `h1`, a `p`, and an unordered list that contains three `li` items. You can include any text you want within each element.

**Note**: When rendering multiple elements like this, you can wrap them all in parentheses, but it's not strictly required. Also notice this challenge uses a `div` tag to wrap all the child elements within a single parent element. If you remove the `div`, the JSX will no longer transpile. Keep this in mind, since it will also apply when you return JSX elements in React components.

---

## Tips

- The constant `JSX` should return a `div` element.

- The `div` should contain a `p` tag as the second element.

- The `div` should contain a `ul` tag as the third element.

- The `div` should contain an `h1` tag as the first element.

- The `ul` should contain three `li` elements.

---

## Solution

```js
// write your code here

const JSX = <div>
        <h1>Título</h1>
        <p>Texto</p>
        <ul>
            <li>Item 1</li>
            <li>Item 2</li>
            <li>Item 3</li>
        </ul>
    </div>;
```