# Arrow Function

We can shorten functions using arrow functions

```javascript
const square = function(num){
    return num*num;
}

// Make it shorter into

const squareArrowFunction = (num) =>{
    return num*num;
} 

// Make it even more shorter

const squareAF = (num) => (num*num);
```

This example shows the advantage of arrow functions and how we can shorten the function declaration

```javascript
const jobs = [
  { id: 1, isActive: true },
  { id: 2, isActive: true },
  { id: 3, isActive: false },
];

const activeJob = jobs.filter((job) => job.isActive);
console.log(activeJob);
```

Output:
```
[ { id: 1, isActive: true }, { id: 2, isActive: true } ]
```
