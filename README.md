# esmoduleinterop-runtime-error

A project which demonstrates a runtime error when using the `esModuleInterop` TypeScript compiler option.

To test, run `npm install` then `npm test`.

```
$ npm install
added 1 package from 1 contributor and audited 1 package in 1.064s
found 0 vulnerabilities

$ npm test

> esmoduleinterop-runtime-error@1.0.0 test C:\Source\node\esmoduleinterop-runtime-error
> tsc --build && node .

lib_1.default.greet();
              ^

TypeError: Cannot read property 'greet' of undefined
    at Object.<anonymous> (C:\Source\node\esmoduleinterop-runtime-error\app\index.js:7:15)
    at Module._compile (internal/modules/cjs/loader.js:689:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:700:10)
    at Module.load (internal/modules/cjs/loader.js:599:32)
    at tryModuleLoad (internal/modules/cjs/loader.js:538:12)
    at Function.Module._load (internal/modules/cjs/loader.js:530:3)
    at Function.Module.runMain (internal/modules/cjs/loader.js:742:12)
    at startup (internal/bootstrap/node.js:283:19)
    at bootstrapNodeJSCore (internal/bootstrap/node.js:743:3)
npm ERR! Test failed.  See above for more details.
```
