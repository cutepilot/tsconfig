## `@esarj/tsconfig`

Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for Eşarj projects.

This module embraces:
- ESM
- Node v12+
- ES2019, ES2020

***Note**: When clonning to your local, place this project under `/@esarj/modules` directory.*

### Installation

```
$ npm install --save-dev github:esarj/tsconfig
```

### Usage

`tsconfig.json`

```jsonc
{
    "extends": "@esarj/tsconfig",
    "compilerOptions": {
        "baseUrl": ".",
        "declarationDir": "lib",
        "outDir": "lib",
        // ...
    },
    // ...
}
```

When you are targeting a higher version of Node.js, check the relevant ECMAScript version and add it as `target`:

```jsonc
{
    "extends": "@esarj/tsconfig",
    "compilerOptions": {
        "target": "ES2021",
        // ...
    },
    // ...
}
```

### Related @esarj projects
- [`@esarj/eslint-config`](https://github.com/esarj/eslint-config) *(Use this instead of `tslint`.)*
