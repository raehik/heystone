# Heystone - Haskell bindings for the Keystone assembler framework
[keystone-gh]: https://github.com/keystone-engine/keystone
[keystone-gh-hs]: https://github.com/keystone-engine/keystone/tree/master/bindings/haskell
[hapstone-gh]: https://github.com/ibabushkin/hapstone

Haskell bindings for [Keystone][keystone-gh], a powerful multi-architecture
assembler framework.

This package is derived from the Haskell bindings at
[keystone-engine/keystone][keystone-gh-hs], which at the time were highly usable
but unmaintained and never uploaded to Hackage. To not obstruct a potential
future official package (and to give myself flexibility), I'm appropriating
[Hapstone][hapstone-gh]'s naming convention.

## Usage
Specify as a dependency in your Cabal file (or Stack, but you'll have to
register it as an `extra-dep`).

You will need the Keystone engine installed. It's not packaged on many systems,
so you many wish to check the [Keystone
docs](https://www.keystone-engine.org/docs/) for instructions. For my fellow
Arch Linux fiends, it's in the main repos:

    pacman -S keystone

## Examples
To build a sample (after having built and installed the Haskell bindings):

```
$ cd bindings/haskell
$ ghc --make samples/Sample.hs
```
