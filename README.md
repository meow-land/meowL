<div align="center">

# meowL

A low-level, statically typed, compiled general-purpose programming language.

</div>

---

## Status

This repository is where meowL will be published as it becomes ready — the language itself, its standard library, examples, and documentation. Nothing here should be considered final until a tagged release says otherwise.

---

## What meowL is

meowL is a systems-level language built around a simple idea: reading and writing code shouldn't require choosing between clarity and control. The syntax stays close to what's already familiar — no semicolons, explicit imports, readable keywords instead of symbol clutter — while the language underneath compiles straight to native machine code, with no hidden runtime standing between the source and the hardware it runs on.

A few things that shape the language:

- **No libc dependency by default.** Programs talk to the operating system directly, through explicit syscalls — nothing is pulled in that wasn't asked for.
- **Memory safety without a heavyweight borrow checker.** Scope-based lifetimes and arena allocation catch common mistakes at compile time, aiming for most of the practical safety with a fraction of the complexity.
- **Cross-architecture inline assembly.** A single `asm` block can target x86_64, ARM64, and RISC-V through one shared syntax, mapped correctly to each platform's calling convention.
- **A type system that stays out of the way until it matters.** Non-nullable pointers by default, traits composed explicitly, generics without runtime overhead.

---

## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE))
- MIT license ([LICENSE-MIT](LICENSE-MIT))

at your option.
