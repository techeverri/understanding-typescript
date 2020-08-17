# 22. Union Types

A union type describes a value that can be one of several types. We use the
vertical bar (`|`) to separate each type, so `number | string | boolean` is the
type of a value that can be a `number`, a `string`, or a `boolean`.

```ts
function combine(a: number | string, b: number | string) {
  return a + b;
}

const combinedAges = combine(29, 31);
console.log(combinedAges); // 60

const combinedNames = combine("Rick", "& Morty");
console.log(combinedNames); // "Rick & Morty"
```

## Links

- [Union Types](https://www.typescriptlang.org/docs/handbook/unions-and-intersections.html#union-types)
