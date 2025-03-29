# Zoodle

**Zoodle** is a compiler for a minimalist Toy Language written in [Zig](https://ziglang.org). It compiles source code into [WebAssembly (WASM)](https://webassembly.org/), with a focus on understanding low-level systems programming, memory management, concurrency, and compiler internals.

This project is educational and hands-on — not just a compiler, but a complete deep dive into modern systems programming with Zig.

---

## 🚀 Project Goals

- Build a real compiler from scratch using Zig
- Learn memory allocation, concurrency, and binary encoding
- Output real `.wasm` binaries that run in browsers and WASM runtimes

---

## 🧩 Toy Language Features

The Toy Language is intentionally small but expressive. It supports:

- `int`, `boolean`, and `string` types
- Immutable variables using `let`
- Arithmetic and logical expressions
- Functions with typed parameters and return values
- Control flow: `if`, `while`, `return`
- Entry point: `fn main() -> int`

Example program:

```tl
fn add(a: int, b: int) -> int {
  return a + b;
}

fn main() -> int {
  let result: int = add(3, 4);
  return result;
}
```

---

## 📦 Compiler Pipeline

Zoodle's compilation steps:

1. **Lexing** – Breaks source code into tokens
2. **Parsing** – Converts tokens to an Abstract Syntax Tree (AST)
3. **Semantic Analysis** – Validates types and scoping
4. **IR Generation** – Produces an intermediate representation
5. **WASM Codegen** – Converts IR into `.wasm` binary
6. **CLI / REPL** – Runs and interacts with the compiled code

---

## 🔧 Technologies

- [Zig](https://ziglang.org) – Systems programming language
- [WebAssembly (binary + WAT format)](https://webassembly.org/)
- Custom parser, memory allocators, and concurrency features

---

## 📚 Documentation

- [Evaluating C, C++, Rust, and Zig for Modern Low-Level Development (Design Philosophies)](https://helabenkhalfallah.com/2025/03/13/evaluating-c-cpp-rust-and-zig-for-modern-low-level-development/)
- [Evaluating C, C++, Rust, and Zig for Modern Low-Level Development (Memory Management)](https://helabenkhalfallah.com/2025/03/15/evaluating-c-c-rust-and-zig-for-modern-low-level-development-memory-management/)
- [Evaluating C, C++, Rust, and Zig for Modern Low-Level Development (Concurrency Mechanisms)](https://helabenkhalfallah.com/2025/03/15/evaluating-c-c-rust-and-zig-for-modern-low-level-development-concurrency-mechanisms/)
- [Evaluating C, C++, Rust, and Zig for Modern Low-Level Development (Error Handling)](https://helabenkhalfallah.com/2025/03/15/evaluating-c-c-rust-and-zig-for-modern-low-level-development-error-handling/)
- [Evaluating C, C++, Rust, and Zig for Modern Low-Level Development (Developer Experience, Portability, Benchmarks and Adoption)](https://helabenkhalfallah.com/2025/03/15/evaluating-c-c-rust-and-zig-for-modern-low-level-development-dx-portability-benchmarks-and-adoption/)

---

## 🤝 Contributing

This is a learning-focused project. Contributions, bug reports, and questions are welcome! Just open an issue or a pull request.

---

## 📄 License

MIT License. See `LICENSE` file for details.

