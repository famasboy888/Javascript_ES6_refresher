# This

When we call `this`, it only references to the Object it was called from

```javascript
const person = {
  name: "John",
  walk() {
    console.log(this)
  },
};

person.walk();
```

```sh
{ name: 'John', walk: [Function: walk] }
```
