# libloading

A memory-safer wrapper around system dynamic library loading primitives. The most important safety
guarantee by this library is prevention of dangling-`Symbol`s that may occur after a `Library` is
unloaded.

Using this library allows loading dynamic libraries (also known as shared libraries) as well as use
functions and static variables these libraries contain.

* [Documentation][docs]
* [Changelog][changelog]

[docs]: https://docs.rs/libloading/
[changelog]: https://docs.rs/libloading/*/libloading/changelog/index.html

libloading is distributed under ISC (MIT-like) license.

## Changes in this fork

This fork adds RcLibrary and RcSymbol which are reference counted pointers to the underlying Libraries and Symbols. Lifetime specifiers can be avoided when using this fork.
