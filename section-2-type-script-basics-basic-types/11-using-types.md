# 11. Using Types

TypeScript supports the same types as JavaScript.<br> _Note: the type system
only works during development_

## [Basic Types](https://www.typescriptlang.org/docs/handbook/basic-types.html)

### [Boolean](https://www.typescriptlang.org/docs/handbook/basic-types.html#boolean)

```ts
let isDone: boolean = false;
```

### [Number](https://www.typescriptlang.org/docs/handbook/basic-types.html#number)

```ts
let decimal: number = 6;
let hex: number = 0xf00d;
let binary: number = 0b1010;
let octal: number = 0o744;
let big: bigint = 100n;
```

### [String](https://www.typescriptlang.org/docs/handbook/basic-types.html#string)

```ts
let color: string = "blue";
let sentence: string = `Hello, my name is ${fullName}.`;
```
