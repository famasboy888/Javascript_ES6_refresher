# Classes

When we have an object with at least 1 method inside it, we need to make a blueprint to create object of that type. 

We will use `class` to create blue prints.

```javascript
class Person {
  constructor(name){
    this.name = name;
  }

  walk() {
    console.log(`${this.name} is walking.`);
  }
}

const person = new Person('Batman');
person.walk();
```

Output:
```
Batman is walking.
```
