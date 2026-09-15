# WebAssembly Extension Docs

Written by AndrewGaming587

### Warning: You should have decent knowledge of both WebAssembly and Javascript before using this extension. The Javascript V2 extension is heavily recommended to be installed and unsandboxed. 

This WebAssembly Extension is intended to be an extension used to allow PenguinMod projects to use the power of WebAssembly (WASM) in a way nearly identical to how you would use WASM in Javascript. Therefore, if you want to learn more about WebAssembly, it is highly recommended that you use [the WASM MDN docs](https://developer.mozilla.org/en-US/docs/WebAssembly) as this documentation is not to teach you about WASM, rather help explain the stuff that won't be in the MDN docs and also what everything would map to in terms of the blocks.

## Dependencies

This extension requires jwklong's Arrays extension, dogeiscut's Objects extension, and my Array Buffers extension, all of which this extension will automatically add, and the Javascript V2 extension unsandboxed, and also jwklong's Integers extension if you plan to deal with any BigInts that may be required or output by any of the blocks, are both suggested but not automatically added.

## Custom Types

This extension has a plethora of custom types, most of them correspond to different classes inside of the `WebAssembly` object in JS.

### Module
Corresponds to a WebAssembly.Module.
To get one, use 
```scratch
create new module [Array Buffer here]::reporter #644fef
```
(where 'Array Buffer here' is an array buffer containing a WASM file)

which is equivalent to 
```js
WebAssembly.compile(arrayBuffer)
```
in JS.

