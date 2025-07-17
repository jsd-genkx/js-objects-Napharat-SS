# JavaScript Objects

## Object Syntax

```js
Syntax:

const objectName = {
  key: value,
  methodName() {
    console.log(this.key);
  }
};

```

## Optional Chaining & Nullish Coalescing Operator

```js
Syntax: obj?.nestedKey;

obj.key ?? defaultValue;
```

## Access Object Properties

- Dot Notation

```js
Syntax: obj.key;
```

- Bracket Notation

```js
Syntax: obj["key"];
```

## --> ADD More Note Here <--

## ADD/UPDATE/DELETE

```js
syntax: 
  obj.newKey = "value";
  obj.existingKey = "updated value";
  delete obj.keyToDelete;
```

## Check If Property Exists
```js
Syntax: 
  "key" in obj
  obj.hasOwnProperty("key");
```
## Loop Through Object

- For In Loop

```js 
Syntax:
  for (let key in obj) {
  console.log(key, obj[key]);
}
```

- Object.keys, Object.values, Object.entries
```js
Syntax:
  const keys = Object.keys(obj);
  const values = Object.values(obj);
  const entries = Object.entries(obj);
```
## Object Destructuring

```js
Syntax:
  const { key1, key2 } = obj;
  const { key: aliasName, missingKey = "default" } = obj;
```

## Nested Destructuring

```js
Syntax:
  const {
  nested: {
    innerKey
  }
} = obj;
```

## Spread Operator (...) with Objects

```js
Syntax:
  const copy = { ...original };
  const merged = { ...obj1, ...obj2 };
```
## Deep Copy
- Modern way (structuredClone - supported in most browsers)
```js
Syntax: const deepCopy = structuredClone(obj);
```

- Alternative (not perfect for all cases)
```js
Syntax: const deepCopy = JSON.parse(JSON.stringify(obj));
```

## Object Methods

```js
Syntax: const person = {
  name: "Yeen",
  greet() {
    console.log(`Hi, I'm ${this.name}`);
  }
};

person.greet();
```

## Object.freeze() vs Object.seal()

```js
Syntax: 
  Object.freeze(obj);
  Object.seal(obj);
```




