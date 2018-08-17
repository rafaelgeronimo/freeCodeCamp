# Profile Lookup

We have an array of objects representing different people in our contacts lists.

A `lookUpProfile` function that takes `name` and a property (`prop`) as arguments has been pre-written for you.

The function should check if `name` is an actual contact's `firstName` and the given property (`prop`) is a property of that contact.

If both are true, then return the "value" of that property.

If `name` does not correspond to any contacts then return `"No such contact"`

If `prop` does not correspond to any valid properties of a contact found to match `name` then return `"No such property"`

---

## Tips

- `"Kristian", "lastName"` should return `"Vos"`

- `"Sherlock", "likes"` should return `["Intriguing Cases", "Violin"]`

- `"Harry","likes"` should return an array

- `"Bob", "number"` should return "No such contact"

- `"Bob", "potato"` should return "No such contact"

- `"Akira", "address"` should return "No such property"

---

## Solution

```js
//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
// Only change code below this line
var quantidade = (contacts.length + 1);
for (var i = 0; i <= quantidade; i++){
    if (i == (quantidade-1)){
        return "No such contact";
    } else if (contacts[i].firstName === name){
        if (contacts[i].hasOwnProperty(prop)){
            return contacts[i][prop];
        }else {
            return "No such property";
        }
    }
}
// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```