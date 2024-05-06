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
const greater100Chars = characters.map( (character) =>{
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
const greater100Chars = characters.map((character) => {
  return character.name.split(" ")[0];
});
```

Output
```javascript
[ 'Luke', 'Darth', 'Leia', 'Anakin' ]
```
