# 21. The "any" type

In some situations, not all type information is available or its declaration
would take an inappropriate amount of effort. These may occur for values from
code that has been written without TypeScript or a 3rd party library. In these
cases, we might want to opt-out of type checking. To do so, we label these
values with the `any` type:

```ts
declare function getValue(key: string): any;

// OK, return value of 'getValue' is not checked
const str: string = getValue("myString");
```

The any type is a powerful way to work with existing JavaScript, allowing you to
gradually opt-in and opt-out of type checking during compilation.

_After all, remember that all the convenience of any comes at the cost of losing
type safety. Type safety is one of the main motivations for using TypeScript and
you should try to avoid using `any` when not necessary._

## Links

- [Any](https://www.typescriptlang.org/docs/handbook/basic-types.html#any)
