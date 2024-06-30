## `@cutepilot/tsconfig`

Common [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for CutePilot projects.

This module embraces:
- ESM
- Node v20+
- ES2021, ESNext

***Note**: When clonning to your local, place this project under `/@cutepilot/modules` directory.*

### Installation

```
$ npm install --save-dev github:cutepilot/tsconfig
```

### Usage

`tsconfig.json`

```jsonc
{
    "extends": "@cutepilot/tsconfig",
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
    "extends": "@cutepilot/tsconfig",
    "compilerOptions": {
        "target": "ES2021",
        // ...
    },
    // ...
}
```

### Related @cutepilot projects
- [`@cutepilot/eslint-config`](https://github.com/cutepilot/eslint-config) *(Use this instead of `tslint`.)*
