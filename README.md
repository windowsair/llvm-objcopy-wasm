# llvm-objcopy-wasm

A port of llvm-objcopy to WebAssembly.

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

[example/convert-to-binary.html](example/convert-to-binary.html)