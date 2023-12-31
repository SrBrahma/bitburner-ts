<div align="center">

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![TypeScript](https://badgen.net/npm/types/env-var)](http://www.typescriptlang.org/)
[![npm](https://img.shields.io/npm/v/bitburner-ts)](https://www.npmjs.com/package/bitburner-ts)
[![npm](https://img.shields.io/npm/dw/bitburner-ts)](https://www.npmjs.com/package/bitburner-ts)

</div>

# bitburner-ts

Rework of [bitburner-filesync](https://github.com/bitburner-official/bitburner-filesync) to work directly with Typescript and with a cleaner implementation. Also, supports WSL when the gaming is running on Windows.

Just run `npx bitburner-ts`! You don't need any special setup in your Typescript project to have this working, like [typescript-template](https://github.com/bitburner-official/typescript-template).

This will automatically set up Typescript on watch mode and will push the resulting .js files into Bitburner. Requires `outDir` and `rootDir` on `tsconfig.json` to be set.

The .js files will be by default put into the `script` directory in the game's `home` server.

You can install it via `npm i bitburner-ts` and have it as a start script in your package.json for quality of life ✨

## Usage

```bash
npx bitburner-ts [options]
# or
npm i bitburner-ts
```

```
Options:
  -p, --port <number>  the port to be used (default: 12525)
  -d, --dest <dir>     directory in the game's home server to put the files (default: "scripts")
  -h, --help           display help for command
```
