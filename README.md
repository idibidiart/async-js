Asynchronous javascript code with different paradigms

# [Synchronous style](https://github.com/nin-jin/async-js/compare/sync?diff=unified&name=sync)

* [+] Very easy logic.
* [+] Easy to support.
* [--] No parallelism.
* [--] Can not be isomorphic in general.

## Start
```sh
npm test
```

## Logic

Controller (index.js) gets user info from model (user.js) and calls view (greeter.js) to talk with user.

# Asynchronous

## Logic

We want to load user info asynchronously. Let's do it with..

## [NodeJS style](https://github.com/nin-jin/async-js/compare/sync...async-nodejs?diff=split&name=async-nodejs)

* [--] Non clear logic. 
* [--] Too more code.
* [--] Need to rewrite all functions.
* [--] Hard to support.
* [--] Hard parallelism.
* [+] Can be isomorphic.

## [Promises style](https://github.com/nin-jin/async-js/compare/sync...async-promises)

* [--] Need to rewrite all functions.
* [--] Hard to support.
* [+] Easy parallelism.
* [+] Can be isomorphic.

## Generators

## async/await

## [Fibers&Futures style](https://github.com/nin-jin/async-js/compare/sync...async-fibers)

* [*] Need to start application in fiber.
* [+] Need not to rewrite all funcitons.
* [+] Easy to support.
* [+] Easy parallelism.
* [--] Can not be isomorphic (NodeJS only).

## [Fibers&Proxies style](https://github.com/nin-jin/async-js/compare/sync...async-fibers-proxy)

* [*] Need to start application in fiber
* [+] Need not to rewrite all funcitons.
* [+] Easy to support.
* [+] Very easy parallelism.
* [--] Can not be isomorphic (NodeJS only).

[More info](https://github.com/nin-jin/node-jin#sod)

## [Atoms style](https://github.com/nin-jin/async-js/compare/sync...async-atoms)

* [--] Need to convert application from control-flow to data-flow.
* [+] Need not to rewrite all funcitons.
* [*] Medium to support.
* [+] Easy parallelism.
* [+] Can be isomorphic.

[More info (russian)](https://habrahabr.ru/post/235121/)
