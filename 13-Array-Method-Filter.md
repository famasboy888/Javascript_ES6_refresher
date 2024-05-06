# Array Method - Filter

## `filter`: Returns a new array with the filtered data

```javascript
const greater100Chars = characters.filter( (character) =>{
  return character.gender === 'male';
});
```

## `map`: Returns a new formed array that is selected in the callback function

Get name and height

```javascript
const nameHeight = characters.map( (character) =>{
  return {
    name: character.name,
    height: character.height,
  };
});
```

Output
```javascript
[
  { name: 'Luke Skywalker', height: '172' },
  { name: 'Darth Vader', height: '202' },
  { name: 'Leia Organa', height: '150' },
  { name: 'Anakin Skywalker', height: '188' }
]
```

Get first names only

```javascript
const firstNames = characters.map((character) => {
  return character.name.split(" ")[0];
});
```

Output
```javascript
[ 'Luke', 'Darth', 'Leia', 'Anakin' ]
```

## `some`: Determines if function meets some certain condition: `true` or `false`

```javascript
const oneMale = characters.some((character) => {
  return character.gender === "male";
});
```

Output
```javascript
true
```

## `sort`:

If the result is negative, `a` is sorted before `b`.

If the result is positive, `b` is sorted before `a`.

```javascript
const sortByMass = characters.sort((a, b) => {
  return (a.gender === "female") ? -1 : 1;
});
```

Output
```javascript
female
male
male
male
```

## `reduce`: Iterate through array and get an ending result

Add all mass in the array

```javascript
const totalMass = characters.reduce((accumulator, currentValue) => {
  return accumulator + parseInt(currentValue.mass);
}, 0);
```

Output:
```
346
```

## `every`: checks if every object in array meets the condition: `true` or `false`

```javascript
const allBlueEyes = characters.every((character) => {
  return character.eye_color === 'blue';
});
```

```
false
```
