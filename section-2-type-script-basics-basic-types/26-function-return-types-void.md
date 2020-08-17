# 26. Function Return Types & "void"

## Return Type Annotations

You can also add return type annotations. Return type annotations appear after
the parameter list:

```ts
function getFavoriteNumber(): number {
  return 7;
}
```

## Void

`void` is a little like the opposite of `any`: the absence of having any type at
all. You may commonly see this as the return type of functions that do not
return a value:

```ts
function warnUser(): void {
  console.log("This is my warning message");
}
```

## Links

- [Return Type Annotations](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#return-type-annotations)
- [Function Types](https://www.typescriptlang.org/docs/handbook/functions.html#function-types)
- [Void](https://www.typescriptlang.org/docs/handbook/basic-types.html#void)
