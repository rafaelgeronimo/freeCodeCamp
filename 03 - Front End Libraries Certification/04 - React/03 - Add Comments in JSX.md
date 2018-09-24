# Add Comments in JSX

JSX is a syntax that gets compiled into valid JavaScript. Sometimes, for readability, you might need to add comments to your code. Like most programming languages, JSX has its own way to do this.

To put comments inside JSX, you use the syntax `{/* */}` to wrap around the comment text.

---

## Challenge

The code editor has a JSX element similar to what you created in the last challenge. Add a comment somewhere within the provided `div` element, without modifying the existing `h1` or `p` elements.

---

## Tips

- The constant `JSX` should return a `div` element.

- The `div` should contain an `h1` tag as the first element.

- The `div` should contain a `p` tag as the second element.

- The `JSX` should include a comment.

---

## Solution

```js
const JSX = (
  <div>
    {/* Isso é um comentário */}
    <h1>This is a block of JSX</h1>
    <p>Here's a subtitle</p>
  </div>
);
```