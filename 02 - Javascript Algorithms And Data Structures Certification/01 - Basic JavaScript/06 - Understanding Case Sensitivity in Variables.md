# Understanding Case Sensitivity in Variables

In JavaScript all variables and function names are case sensitive. This means that capitalization matters.

`MYVAR` is not the same as `MyVar` nor `myvar`. It is possible to have multiple distinct variables with the same name but different casing. It is strongly recommended that for the sake of clarity, you *do not* use this language feature.

Best Practice

Write variable names in JavaScript in *camelCase*. In *camelCase*, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.

**Examples**:

```js
var someVariable;
var anotherVariableName;
var thisVariableNameIsSoLong;
```

---

## Challenge

Modify the existing declarations and assignments so their names use *camelCase*.
Do not create any new variables.

---

## Tips

- `studlyCapVar` is defined and has a value of `10`

- `properCamelCase` is defined and has a value of `"A String"`

- `titleCaseOver` is defined and has a value of `9000`

- `studlyCapVar` should use camelCase in both declaration and assignment sections.

- `properCamelCase` should use camelCase in both declaration and assignment sections.

- `titleCaseOver` should use camelCase in both declaration and assignment sections.

---

## Solution

```js
// Declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```