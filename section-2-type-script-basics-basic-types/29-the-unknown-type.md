# 29. The "unknown" Type

We may need to describe the type of variables that we do not know when we are
writing an application. These values may come from dynamic content - e.g. from
the user - or we may want to intentionally accept all values in our API. In
these cases, we want to provide a type that tells the compiler and future
readers that this variable could be anything, so we give it the unknown type.

```ts
let notSure: unknown = 4;
notSure = "maybe a string instead";

// OK, definitely a boolean
notSure = false;
```

## Links

- [Unknown](https://www.typescriptlang.org/docs/handbook/basic-types.html#unknown)
