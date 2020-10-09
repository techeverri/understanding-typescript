# 36. Including & Excluding Files

## `include`

Specifies an array of filenames or patterns to include in the program. These
filenames are resolved relative to the directory containing the `tsconfig.json`
file.

```json
{
  "include": ["src/**/*", "tests/**/*"]
}
```

Which would include:

```text
.
├── scripts                ⨯
│   ├── lint.ts            ⨯
│   ├── update_deps.ts     ⨯
│   └── utils.ts           ⨯
├── src                    ✓
│   ├── client             ✓
│   │    ├── index.ts      ✓
│   │    └── utils.ts      ✓
│   ├── server             ✓
│   │    └── index.ts      ✓
├── tests                  ✓
│   ├── app.test.ts        ✓
│   ├── utils.ts           ✓
│   └── tests.d.ts         ✓
├── package.json
├── tsconfig.json
└── yarn.lock
```

## `exclude`

`exclude` specifies an array of filenames or patterns that should be skipped
when resolving `include`.

**Important**: `exclude` only changes which files are included as a result of
the `include` setting. A file specified by `exclude` can still become part of
your codebase due to an `import` statement in your code, a `types` inclusion, a
`/// <reference` directive, or being specified in the `files` list.

It is not a mechanism that prevents a file from being included in the codebase -
it simply changes what the include setting finds.

## wildcards

`include` and `exclude` support wildcard characters to make glob patterns:

- `*` matches zero or more characters (excluding directory separators)
- `?` matches any one character (excluding directory separators)
- `**/` matches any directory nested to any level

If a glob pattern doesn't include a file extension, then only files with
supported extensions are included (e.g. `.ts`, `.tsx`, and `.d.ts` by default,
with `.js` and `.jsx` if `allowJs` is set to true).

## Links

- [TSConfig Reference / File Inclusion](https://www.typescriptlang.org/tsconfig#Project_Files_0)
- [Why does a module in the exclude list still get picked up by the compiler?](https://www.typescriptlang.org/docs/handbook/module-resolution.html#why-does-a-module-in-the-exclude-list-still-get-picked-up-by-the-compiler)
