# 18. Array Types

TypeScript, like JavaScript, allows you to work with arrays of values. Array
types can be written in one of two ways. In the first, you use the type of the
elements followed by `[]` to denote an array of that element type:

```ts
let list: number[] = [1, 2, 3];
```

The second way uses a generic array type, `Array<elemType>`:

```ts
let list: Array<number> = [1, 2, 3];
```

## Examples

### Array of strings

```ts
let hobbies: string[];

hobbies = ["Volleyball", "Badminton", "Football"];
```

### Array of whatever

```ts
let whatever: any[]; // let whatever: Array<any>;

whatever = ["Hello", true, {}, 7];
```

All the convenience of any comes at the cost of losing type safety. Type safety
is one of the main motivations for using TypeScript and you should try to avoid
using any when not necessary.

## Links

- [Array](https://www.typescriptlang.org/docs/handbook/basic-types.html#array)
- [Any](https://www.typescriptlang.org/docs/handbook/basic-types.html#any)
