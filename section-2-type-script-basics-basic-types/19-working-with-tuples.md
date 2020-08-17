# 19. Working with Tuples

Tuple types allow you to express an array with a fixed number of elements whose
types are known, but need not be the same. For example, you may want to
represent a value as a pair of a `string` and a `number`:

```ts
let response: [number, string];

response = [502, "Bad Gateway"];
```

When accessing an element with a known index, the correct type is retrieved:

```ts
response[1].toUpperCase();
```

Accessing an element outside the set of known indices fails with an error:

```ts
response[0].toUpperCase();
```

## Links

- [Tuple](https://www.typescriptlang.org/docs/handbook/basic-types.html#tuple)
