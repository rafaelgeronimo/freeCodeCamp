# Access Props Using this.props

The last several challenges covered the basic ways to pass props to child components. But what if the child component that you're passing a prop to is an ES6 class component, rather than a stateless functional component? The ES6 class component uses a slightly different convention to access props.

Anytime you refer to a class component within itself, you use the `this` keyword. To access props within a class component, you preface the code that you use to access it with `this`. For example, if an ES6 class component has a prop called data, you write `{this.props.data}` in JSX.

---

## Challenge

Render an instance of the `ReturnTempPassword` component in the parent component `ResetPassword`. Here, give `ReturnTempPassword` a prop of `tempPassword` and assign it a value of a string that is at least 8 characters long. Within the child, `ReturnTempPassword`, access the `tempPassword` prop within the `strong` tags to make sure the user sees the temporary password.

---

## Tips

- The `ResetPassword` component should return a single `div` element.

- The fourth child of `ResetPassword` should be the `ReturnTempPassword` component.

- The `ReturnTempPassword` component should have a prop called `tempPassword`.

- The `tempPassword` prop of `ReturnTempPassword` should be equal to a string of at least 8 characters.

- The `ReturnTempPassword` component should display the password you create as the `tempPassword` prop within `strong` tags.

---

## Solution

```js
class ReturnTempPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
            { /* change code below this line */ }
            <p>Your temporary password is: <strong>{this.props.tempPassword}</strong></p>
            { /* change code above this line */ }
        </div>
    );
  }
};

class ResetPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
          <h2>Reset Password</h2>
          <h3>We've generated a new temporary password for you.</h3>
          <h3>Please reset this password from your account settings ASAP.</h3>
          { /* change code below this line */ }
            <ReturnTempPassword tempPassword= {"12345678"}/>
          { /* change code above this line */ }
        </div>
    );
  }
};
```