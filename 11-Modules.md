# Modules

`modules` are when we separate each definitions in their own separate files. This is called **modularity**.

We moved files in their own separate files.

main.js
```javascript
import { Teacher } from "./teacher.js";

const teacher = new Teacher("Smith", "Math");
teacher.teach();
teacher.walk();

```

teacher.js
```javascript
import { Person } from "./person.js";

export class Teacher extends Person {
  constructor(name, degree) {
    super(name);
    this.degree = degree;
  }
  teach() {
    console.log(`${this.name} will teach with degree of ${this.degree}!`);
  }
}
```

person.js
```javascript
export class Person {
  constructor(name) {
    this.name = name;
  }

  walk() {
    console.log(`${this.name} is walking.`);
  }
}
```
