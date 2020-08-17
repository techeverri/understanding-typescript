# 15. Type Assignment & Type Inference

## Good practice ✅

- Add basic types to uninitialized variables<br/> _Please the compiler what to
  expect in the future_

```ts
const amount: number;
```

## Bad practice ❌

- Add basic types to initialized variables<br> _The type inference will take
  care of it_

```ts
const amount: number = 7;
```
