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


## Team Members

 1. [Manohar Pattanayak](https://github.com/manoharbabun)
 2. [Srijan Paul](https://github.com/srijan-paul/)
