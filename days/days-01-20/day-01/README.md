# Day 1 — Rust (100 Days)

**Date:** 12/28/25

Welcome! This is the start of a 100-day Rust learning journey. Each day you'll get short notes, key concepts, commands to try, and links to resources.

## Day 1 — Overview

Today you'll:

- Install Rust using `rustup`.
- Create a new Cargo project.
- Run your first "Hello, World!" program.

By the end of today you'll have a working Rust project and a basic understanding of `rustc`, `cargo`, and the development workflow.

## What is Rust?

Rust is a modern systems programming language focused on performance, reliability, and safety. It prevents common bugs (null dereferences, data races, buffer overflows) using the ownership system, the borrow checker, and a strong type system at compile time. Rust is well suited for WebAssembly, embedded systems, CLI tools, and replacing C/C++ in performance-critical code.

If you come from C++, Python, or JavaScript, Rust can feel strict at first, but the rules help you write safer code.

Learn more: The Rust Programming Language — https://doc.rust-lang.org/book/

## Installing Rust

Rust uses `rustup` to install and manage toolchains (stable, beta, nightly). `rustup` installs `rustc`, `cargo`, and other tools.

On macOS or Linux, run:

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Follow the prompts, then reload your shell environment:

```sh
source $HOME/.cargo/env
rustc --version
```

On Windows, use the installer listed at https://www.rust-lang.org/tools/install and follow the instructions.

If installation succeeds, `rustc --version` should print the compiler version.

## Development Environment

Choose an editor or IDE. Recommended: Visual Studio Code with the `rust-analyzer` extension for auto-completion, diagnostics, and debugging.

Alternatives: IntelliJ IDEA (with Rust plugin), Vim/Neovim, or a simple text editor.

## Your First "Hello, World!" Project

Create and run a new project with Cargo:

```sh
mkdir RustJourney
cd RustJourney
cargo new hello_world
cd hello_world
cargo run
```

Cargo generates:

- `src/main.rs` — main source file
- `Cargo.toml` — project metadata
- `.gitignore` — recommended ignores

Open `src/main.rs`. Cargo pre-fills it with:

```rust
fn main() {
    println!("Hello, world!");
}
```

Explanation:

- `fn main()` — program entry point
- `println!` — macro that prints to stdout (note the `!`)
- Statements end with `;`

Build and run:

```sh
cargo run
```

Build only:

```sh
cargo build
```

Optimized release build:

```sh
cargo build --release
```

## What is Cargo?

Cargo is Rust's build system and package manager. It:

- Creates new projects with a standard layout
- Builds your code (using `rustc` under the hood)
- Manages dependencies (crates) from https://crates.io
- Runs tests, benchmarks, and generates docs
- Packages projects for distribution

Project metadata lives in `Cargo.toml`.

Learn more: https://doc.rust-lang.org/cargo

## Exercises

- Change the printed message to your name.
- Add a small function and call it from `main()`.
- Introduce a compile error intentionally, then fix it and observe the compiler diagnostics.

## Resources

- The Rust Programming Language (book): https://doc.rust-lang.org/book/
- Rust by Example: https://doc.rust-lang.org/rust-by-example/
- Official install guide: https://www.rust-lang.org/learn/get-started

## Summary

- Installed Rust via `rustup`
- Learned what Cargo does
- Created and ran a Hello World project

Happy hacking — welcome to the Rustacean club! 🦀
