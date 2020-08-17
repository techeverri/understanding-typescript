# 23. Literal Types

A literal is a more concrete sub-type of a collective type. What this means is
that `"Hello World"` is a `string`, but a `string` is not `"Hello World"` inside
the type system.

There are three sets of literal types available in TypeScript today: strings,
numbers, and booleans; by using literal types you can allow an exact value which
a string, number, or boolean must have.

## Literal Narrowing

When you declare a variable via `var` or `let`, you are telling the compiler
that there is the chance that this variable will change its contents. In
contrast, using `const` to declare a variable will inform TypeScript that this
object will never change.

```ts
// We're making a guarantee that this variable
// helloWorld will never change, by using const.

// So, TypeScript sets the type to be "Hello World" not string
const helloWorld = "Hello World";

// On the other hand, a let can change, and so the compiler declares it a string
let hiWorld = "Hi World";
```

## String Literal Types

In practice string literal types combine nicely with union types, type guards,
and type aliases. You can use these features together to get enum-like behavior
with strings.

```ts
type Easing = "ease-in" | "ease-out" | "ease-in-out";

declare function animate(easing: Easing) {
  // something
};
```

## Links

- [Literal Types](https://www.typescriptlang.org/docs/handbook/literal-types.html)
- [String Literal Types](https://www.typescriptlang.org/docs/handbook/literal-types.html#string-literal-types)
- [Numeric Literal Types](https://www.typescriptlang.org/docs/handbook/literal-types.html#numeric-literal-types)
- [Boolean Literal Types](https://www.typescriptlang.org/docs/handbook/literal-types.html#boolean-literal-types)
