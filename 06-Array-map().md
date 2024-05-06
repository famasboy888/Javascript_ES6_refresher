# Array.map()

This is commonly used in React to render or loop through a list.

```javascript
const colors = ["red", "green", "blue"];

const items = colors.map((color)=>`<li key="${color}">${color}</li>`);

console.log(items);
```
Output:
```
[
  '<li key="red">red</li>',
  '<li key="green">green</li>',
  '<li key="blue">blue</li>'
]
```
