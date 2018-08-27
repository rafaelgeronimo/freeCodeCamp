# Iterate Through the Keys of an Object with a for...in Statement

Sometimes you may need to iterate through all the keys within an object. This requires a specific syntax in JavaScript called a `for...in` statement. For our `users` object, this could look like:

```js
for (let user in users) {
  console.log(user);
};

// logs:
Alan
Jeff
Sarah
Ryan
```

In this statement, we defined a variable `user`, and as you can see, this variable was reset during each iteration to each of the object's keys as the statement looped through the object, resulting in each user's name being printed to the console.

## NOTE

Objects do not maintain an ordering to stored keys like arrays do; thus a keys position on an object, or the relative order in which it appears, is irrelevant when referencing or accessing that key.

---

## Challenge

We've defined a function, `countOnline`; use a *for...in* statement within this function to loop through the users in the `users` object and return the number of users whose `online` property is set to `true`.

---

## Tips

- The `users` object contains users `Jeff` and `Ryan` with `online` set to `true` and users `Alan` and `Sarah` with `online` set to `false`

- The function `countOnline` returns the number of users with the `online` property set to `true`

---

## Solution

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {
  // change code below this line
    let i = 0;
    for (let user in obj){
        if (users[user].online === true){
            console.log(users[user].online);
            i++;
        }
    }
    return i;
  // change code above this line
}

console.log(countOnline(users));
```