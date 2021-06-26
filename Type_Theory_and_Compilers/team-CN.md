## Project Name
Boa- Static type inference and native compilation for Python

## Domain
Type Theory | Compiler Tooling | Math

## Link

[Boa](https://github.com/srijan-paul/Boa--compiling-python)

## About Project

**Boa** is a static analysis tool for the Python programming language that works without needing
any type annotations. It performs flow sensitive type analysis and and is capable of inferring type 
information from code using [Hindley Milner](https://en.wikipedia.org/wiki/Hindley%E2%80%93Milner_type_system) type inference and a [unification](https://en.wikipedia.org/wiki/Unification_(computer_science)) algorithm.

This project attempts to demonstrate that better tooling is possible for dynamically typed languages without
needing an extra layer of traspilation with superset languages like [Typescript](https://www.typescriptlang.org/) or [Flow](https://flow.org/).

As a bonus, Boa can compile python to native x86 machine code, boosting it's speed by some orders of magnitude.
Boa watches the filesystem for changes in source code and reports errors as soon as it encounters them.

**Tech stack**:

 - Python
 - C
 - x86 ASM
 - Numpy
 - WatchDog
 - Bash


## Team Members
 1. [Manohar Pattanayak](https://github.com/manoharbabun)
 2. [Srijan Paul](https://github.com/srijan-paul/)

## Weekly Progress

### Week 1
- Implemented Parsing, syntax analysis and basic type checking for primitive data types.
- Added a barebones framework for the Hindey Milner unification engine.

### Week 2
- Can now compile basic control flow structures down to assembly instructions.
- Added context sensitive type analysis.
- Implemented a high level IR that acts as a middle ground between the AST and the native machine code.

### Week 3
- Added structural type inference and machine code generation for loops and functions.
- Implemented Type Traits and type classes.
- Wrote unit tests and a CLI tool for on-demand compilation of files.
- Benchmarks comparing execution speeds of of major python implementations like PyPy and CPython with Boa.
- Dead code elemination and constant propagation optimizations.
- Runtime library written in C and linked and loaded using a hand-written loader.

## References
1. [Type traits in Rust](https://doc.rust-lang.org/book/ch10-02-traits.html). Polymorphic types in boa are supported
by allowing type traits inspired from Rust and Haskell.

2. [Stephen Deihl's Hindley Milner Type inference for Haskell](http://dev.stephendiehl.com/fun/006_hindley_milner.html).
We used this E-book as reference for implementing the type equation generation and on-demand constraint solving.

3. [Rescript](https://rescript-lang.org/). An OCaml like programming languge developed as facebook that as similar type inference, but it compiles to Javascript and does not play nice with mutation. We used Rescript's OCaml type-checker (that can be found [here](https://github.com/rescript-lang/ocaml/blob/7d45d126c85c6e1a43260132ac28e2e45f80ce42/typing/typedtree.ml)) as a
reference for adding implicit AST annotations to the parsed Python AST in our type inference engine.