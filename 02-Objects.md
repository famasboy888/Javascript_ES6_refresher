# Objects

### Objects in JS are collection of key and value pairs:

```javascript
const person = {
  name: 'John',
  walk: function() { },         // Old way
  talk() { }                    // new way
}
```

### 2 ways of accessing objects:

If we can pre-determine the value:

```javascript
person.talk();

person.name = '';
```

If we do not know the value:

```javascript
const targetMember = 'name';

person[targetMember.value] = 'Jake';
```
