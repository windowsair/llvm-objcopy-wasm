# llvm-objcopy-wasm

A port of llvm-objcopy to WebAssembly.

# Install

```bash
npm i llvm-objcopy-wasm
```

# Usage

```js
import Module from 'src/llvm-objcopy.mjs'

let handle = await Module()
let args = []
let exitCode = handle.callMain(args)

// See console:

// OVERVIEW: llvm-objcopy tool
//
// USAGE: llvm-objcopy [options] input [output]
//
// ...
```

For more information, see: [llvm-objcopy Document](https://llvm.org/docs/CommandGuide/llvm-objcopy.html)

# Example

## 1. Covert input file to binary format in browser

Equivalent command line:

```bash
llvm-objcopy -O binary input outout
```

Try it online: [convert-to-binary](https://llvm-objcopy-wasm.vercel.app/example/convert-to-binary.html)

Source code: [example/convert-to-binary.html](example/convert-to-binary.html)
