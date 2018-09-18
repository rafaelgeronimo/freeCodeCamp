# Map the Debris

Return a new array that transforms the elements' average altitude into their orbital periods (in seconds).

The array will contain objects in the format `{name: 'name', avgAlt: avgAlt}`.

You can read about orbital periods [on Wikipedia](http://en.wikipedia.org/wiki/Orbital_period).

The values should be rounded to the nearest whole number. The body being orbited is Earth.

The radius of the earth is 6367.4447 kilometers, and the GM value of earth is 398600.4418 km3s-2.

Remember to use Read-Search-Ask if you get stuck. Try to pair program. Write your own code.

---

## Tips

- `orbitalPeriod([{name : "sputnik", avgAlt : 35873.5553}])` should return `[{name: "sputnik", orbitalPeriod: 86400}]`.

- `orbitalPeriod([{name: "iss", avgAlt: 413.6}, {name: "hubble", avgAlt: 556.7}, {name: "moon", avgAlt: 378632.553}])` should return `[{name : "iss", orbitalPeriod: 5557}, {name: "hubble", orbitalPeriod: 5734}, {name: "moon", orbitalPeriod: 2377399}]`.

---

## Solution

```js
function orbitalPeriod(arr) {
  var GM = 398600.4418;
  var earthRadius = 6367.4447;
  var x = 2 * Math.PI;
  var newArr = [];

  var getOrbPeriod = function(obj) {
    var y = Math.pow(earthRadius + obj.avgAlt, 3);
    var z = Math.sqrt(y / GM);
    var orbPeriod = Math.round(x * z);
    delete obj.avgAlt;
    obj.orbitalPeriod = orbPeriod;
    return obj;
  };

  for (var elem in arr) {
    newArr.push(getOrbPeriod(arr[elem]));
  }

  return newArr;
}

//orbitalPeriod([{name : "sputnik", avgAlt : 35873.5553}]);// should return [{name: "sputnik", orbitalPeriod: 86400}].

orbitalPeriod([
  {name: "iss", avgAlt: 413.6}, 
  {name: "hubble", avgAlt: 556.7}, 
  {name: "moon", avgAlt: 378632.553}
]);

/* should return 
[{name : "iss", orbitalPeriod: 5557}, 
{name: "hubble", orbitalPeriod: 5734}, 
{name: "moon", orbitalPeriod: 2377399}].
*/
```