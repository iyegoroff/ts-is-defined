# ts-is-defined

[![npm](https://img.shields.io/npm/v/ts-is-defined)](https://npm.im/ts-is-defined)
[![build](https://github.com/iyegoroff/ts-is-defined/workflows/build/badge.svg)](https://github.com/iyegoroff/ts-is-defined/actions/workflows/build.yml)
[![publish](https://github.com/iyegoroff/ts-is-defined/workflows/publish/badge.svg)](https://github.com/iyegoroff/ts-is-defined/actions/workflows/publish.yml)
![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/npm/ts-is-defined)
[![Bundlephobia](https://img.shields.io/bundlephobia/minzip/ts-is-defined?label=min+gzip)](https://bundlephobia.com/package/ts-is-defined)
[![npm](https://img.shields.io/npm/l/ts-is-defined.svg?t=1495378566925)](https://www.npmjs.com/package/ts-is-defined)

<!-- [![Bundlephobia](https://badgen.net/bundlephobia/minzip/ts-is-defined?label=min+gzip)](https://bundlephobia.com/package/ts-is-defined) -->

Typescript utilities

```ts
export function isDefined<T>(value: T): value is NonNullable<T> {
  return value !== undefined && value !== null
}

export function assertDefined<T>(
  value: T,
  message: string
): asserts value is NonNullable<T> {
  invariant(isDefined(value), message)
}
```
