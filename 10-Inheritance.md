# Inheritance

This allows us to reuse the previous class and inherit it's methods.

```javascript
class Person {
  constructor(name){
    this.name = name;
  }

  walk() {
    console.log(`${this.name} is walking.`);
  }
}


class Teacher extends Person{
  teach(){
    console.log(`${this.name} will teach!`)
  }
}

const teacher = new Teacher('Smith');
teacher.teach();
teacher.walk();
```

Output:
```
Smith will teach!
Smith is walking.
```
