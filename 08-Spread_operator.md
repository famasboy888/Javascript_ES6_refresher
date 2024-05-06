# Spread Operator

```javascript
const firtArr = [1,2,3];
const secondArr = [4,5,6];

// The old way to combine the 2 arrays
const combine = firtArr.concat(secondArr);

// Spread operator
const combineSpread = [...firtArr, ...secondArr];
console.log(combineSpread);
```
output
```
[ 1, 2, 3, 4, 5, 6 ]
```

Another example using objects:

```javascript
const firstObj = { name: "batman" };
const secondObj = { job: "protect city" };

const combine = {...firstObj,...secondObj,city:'Gotham'}

console.log(combine);
```
Output
```
{ name: 'batman', job: 'protect city', city: 'Gotham' }
```
