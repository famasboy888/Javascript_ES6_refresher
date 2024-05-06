# Object Destructuring

We use destructuring in react often to simplify declaration of variables from object.

```javascript
const address = {
  street: "",
  city: "",
  country: "",
};

//Old way
const street = address.street;
const city = address.city;
const country = address.country;

//Destructuring
const { street, city, country } = address;
```

We can also use an `alias`:

```javascript
const { street: st, city: ct, country: cnty } = address;
```
