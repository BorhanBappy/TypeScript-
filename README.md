# Basic TypeScript

```typescript
// deno basic.ts
// Array
let fruits = ["Apple", "banana", "orange"];
// fruits.push(34);
console.log(fruits);

// Object
let person = {
  name: "Marshafi",
  age: 35,
  inCaptain: true,
};
// person.name=34; // error because change the type of variable.

// person.country='Bangladesh'; // error because country not assign in object.
console.log(person);
```

# Explicit & Union Types

```typescript
let a: string;
let b: number;

a = "borhan";
b = 34;
// a=34 finding error
```

## Array

```typescript
let a: string[] = [];
a.push("2");
console.log(a);
// Union Array
let b: (string | number)[] = [];

b.push(2);
b.push("BAppy");

console.log(b);
```

## Object

```typescript
// let c: object;
// c = [12, 10];
// console.log(c);
// c = {
//   name: "Bappy",
//   age: 25,
// };

// console.log(c);
// Object declaration with explicit type
let c: {
  name: string;
  age: number;
  adult: boolean;
};
// c=[] error it except string,number, boolean

c = {
  name: "Bappy",
  age: 25,
  adult: true,
};

/*
but used adult without boolean or name without string  we find error
c = {
  name: "Bappy",
  age: 25,
  adult: "true",
};
*
```
