# 37. Setting a Compilation Target

Modern browsers support all ES6 features, so `ES6` is a good choice. You might
choose to set a lower target if your code is deployed to older environments, or
a higher target if your code is guaranteed to run in newer environments.

The `target` setting changes which JavaScript features are downleveled and which
are left intact. For example, an arrow function `() => this` will be turned into
an equivalent `function` expression if target is ES5 or lower.

Changing `target` also changes the default value of `lib`. You may "mix and
match" `target` and `lib` settings as desired, but you could just set `target`
for convenience.

If you are only working with Node.js, here are recommended `target`s based on
the Node version:

| Name    | Supported Target |
| ------- | ---------------- |
| Node 8  | ES2017           |
| Node 10 | ES2018           |
| Node 12 | ES2019           |

These are based on [node.green](https://node.green/)'s database of support.

The special `ESNext` value refers to the highest version your version of
TypeScript supports. This setting should be used with caution, since it doesn't
mean the same thing between different TypeScript versions and can make upgrades
less predictable.

## Links

- [TSConfig Reference / Target](https://www.typescriptlang.org/tsconfig#target)
- [Node.js ES2015/ES6, ES2016 and ES2017 support](https://node.green/)
