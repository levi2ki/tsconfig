# Collection of TS configs.
> Read more about shareable configuration at [official documentation](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html#tsconfig-bases)

## Installation
```shell
npm i --save-dev @levi2ki/tsconfig
```

## Using
Extend your config with `extends` keyword.
```json
{
  "extends": "@levi2ki/tsconfig/standard",
  "compilerOptions": {
    "baseUrl": "./",
    "typeRoots": ["./src/@types", "node_modules/@types"]
  },
  "include": ["src"],
  "exclude": ["node_modules"]
}
```
> ❗ Do not forget to define specific options `include`, `exclude`, `baseUrl`, `typeRoots`, `rootDir`, `outDir`, `declarationDir` etc and other path specific options as **they will not be shared** via extends

## Available configs
* `react-standard` mostly usual strict config with most important options.
* `react-recommended` recommended config with options, that cover you from most gotchas - use this if you like strict code.
