# Arrow Functions and This

Arrow functions don't rebind `this` keyword. Arrow functions allow inheriting of `this`.

Compare the following outputs:

```javascript
//Old Function implementation

const person = {
  name: "John",
  walk() {
    setTimeout(function() {
        console.log(this);
    })
  },
};

person.walk();
```

Output
```
Timeout {
  _idleTimeout: 1,
  _idlePrev: null,
  _idleNext: null,
  _idleStart: 15,
  _onTimeout: [Function (anonymous)],
  _timerArgs: undefined,
  _repeat: null,
  _destroyed: false,
  [Symbol(refed)]: true,
  [Symbol(kHasPrimitive)]: false,
  [Symbol(asyncId)]: 2,
  [Symbol(triggerId)]: 1
}
```

---

```javascript
//Arrow Function

const person = {
  name: "John",
  walk() {
    setTimeout(()=>{
        console.log(this);
    })
  },
};

person.walk();
```
Output:
```
{ name: 'John', walk: [Function: walk] }
```
