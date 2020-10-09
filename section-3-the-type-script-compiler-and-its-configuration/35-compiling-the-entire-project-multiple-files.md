# 35. Compiling the Entire Project / Multiple Files

Running `tsc` locally will compile the closest project defined by a
`tsconfig.json`, you can compile a set of TypeScript files by passing in a glob
of files you want.

```sh
# Run a compile based on a backwards look through the fs for a tsconfig.json
❯ tsc

# Transpile just the index.ts with the compiler defaults
❯ tsc index.ts

# Transpile any .ts files in the folder src, with the default settings
❯ tsc src/*.ts

# Transpile any files referenced in with the compiler settings from tsconfig.production.json
❯ tsc --project tsconfig.production.json
```

The presence of a `tsconfig.json` file in a directory indicates that the
directory is the root of a TypeScript project. The `tsconfig.json` file
specifies the root files and the compiler options required to compile the
project.

Running `npx tsc --init` initializes a TypeScript project and creates a
`tsconfig.json` file.

## Links

- [`tsc` CLI Options](https://www.typescriptlang.org/docs/handbook/compiler-options.html)
- [What is a tsconfig.json](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html)
- [TSConfig Bases](https://github.com/tsconfig/bases)
