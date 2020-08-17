# 27. Functions as Types

A function's type has two parts: the type of the arguments and the return type.
When writing out the whole function type, both parts are required. We write out
the parameter types just like a parameter list, giving each parameter a name and
a type. This name is just to help with readability. We could have instead
written:

```ts
let myAdd: (baseValue: number, increment: number) => number = function (
  x: number,
  y: number
): number {
  return x + y;
};
```

## Links

- [Writing the function type](https://www.typescriptlang.org/docs/handbook/functions.html#writing-the-function-type)
