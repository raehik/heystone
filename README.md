# Keystone Haskell bindings
[keystone-gh]: https://github.com/keystone-engine/keystone
[keystone-gh-hs]: https://github.com/keystone-engine/keystone/tree/master/bindings/haskell

Haskell bindings for [Keystone][keystone-gh], a powerful multi-architecture
assembler framework.

This package is derived from the Haskell bindings at
[keystone-engine/keystone][keystone-gh-hs], which at the time were highly usable
but unmaintained and never uploaded to Hackage.

## Building
TODO

1. Install the core Keystone Assembler as a dependency:

   Follow docs/COMPILE.md in the root directory to compile & install the core.
2. Change into the Haskell bindings directory, build and install:

    ```
$ cd bindings/haskell
$ cabal install
```

If you are installing into a sandbox, run `cabal sandbox init` before
installing Keystone's dependencies.

If the build fails, install c2hs manually `cabal install c2hs` (note that this
will probably also require you to run `cabal install alex` and `cabal install
happy` as well). If you are NOT using a sandbox, ensure that `$HOME/.cabal/bin`
is on your PATH.

To build a sample (after having built and installed the Haskell bindings):

```
$ cd bindings/haskell
$ ghc --make samples/Sample.hs
```
