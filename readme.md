# `@alwaysai/tsconfig`

TypeScript configurations for alwaysAI projects

## Usage

These instructions assume that you're using TypeScript >=[3.2 with support for "tsconfig.json inheritance via Node.js packages"](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-2.html). 

```
npm install --save-dev typescript @alwaysai/tsconfig
```

Create a file `tsconfig.json` at the root of your project with contents:

```json
{
  "extends": "@alwaysai/tsconfig"
}
```

Add your own `compilerOptions` or any other properties described [here in the TypeScript docs](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html).

The `@alwaysai/tsconfig` [base configuration](tsconfig.json) sets some desirable non-default values such as `"strict": true`. It also enumerates as comments most of the other available configuration options. The base configuration can be used directly as `"extends": "@alwaysai/tsconfig"`. This package also makes available a Node.js-specific configuration usable as `"extends": "@alwaysai/tsconfig/nodejs/tsconfig.json`". The `nodejs` configuration extends the base one and also sets "es2017" as the compiler target, suitable for use with Node.js >=8.

## Related
- [@alwaysai/eslint-config](https://github.com/alwaysai/eslint-config): ESLint configurations for alwaysAI projects

## License
MIT © [alwaysAI, Inc.](https://alwaysai.co)
