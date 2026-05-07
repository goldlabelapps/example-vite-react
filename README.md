# example-vite-react

A raw test harness for [`@goldlabelapps/virus`](https://www.npmjs.com/package/@goldlabelapps/virus) — kept as close to the default bootstrapped scaffold as possible so results are clean and unambiguous.

## Tech stack

| Layer | Choice |
|---|---|
| Bundler | [Vite](https://vitejs.dev) |
| UI library | [React 18](https://react.dev) |
| Language | TypeScript |
| Linting | ESLint 9 (flat config) |

Bootstrapped with:

```bash
npm create vite@latest -- --template react-ts
```

## Purpose

This repo exists solely to test the `@goldlabelapps/virus` npm package in a real React/TypeScript environment. No extra dependencies, no abstractions — just a minimal host app that imports and exercises the package.

## Install the package

```bash
npm i @goldlabelapps/virus
```

## Quick start

```ts
import { renderPackageInfo, PACKAGE_NAME, PACKAGE_VERSION } from '@goldlabelapps/virus';

console.log(renderPackageInfo());
// @goldlabelapps/virus v1.1.0

console.log(PACKAGE_NAME);    // "@goldlabelapps/virus"
console.log(PACKAGE_VERSION); // "1.1.0"
```

## API

### `renderPackageInfo()`

- Returns: `string`
- Format: `<package-name> v<package-version>`

### `PACKAGE_NAME`

- Type: `string`
- Value: `@goldlabelapps/virus`

### `PACKAGE_VERSION`

- Type: `string`
- Value: current published version

## Development

```bash
npm install
npm run dev
```

## Links

- npm: [npmjs.com/package/@goldlabelapps/virus](https://www.npmjs.com/package/@goldlabelapps/virus)
- Source: [github.com/goldlabelapps/virus](https://github.com/goldlabelapps/virus)

---

[MIT](./LICENSE) © Goldlabel°
