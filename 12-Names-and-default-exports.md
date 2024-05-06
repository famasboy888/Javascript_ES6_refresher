# Names and Default Export

We only use `{ }` for importing named exports.

We import directly the name of default exports.

### See examples:

Default -> 

```javascript
import Person from "./person.js";
```

```javascript
export default class Person {
  ...
}
```

Named ->

```javascript
import { Teacher } from "./teacher.js";
```

```javascript
export class Teacher extends Person {
  ...
}
```

Both Named and Default Export ->

```javascript
import Person, {promote} from "./person.js";
```

```javascript
export const promote = () => {
  ...
}

export class Teacher extends Person {
  ...
}
```
