# jBC Language

An unofficial reference guide and an experimental compiler for jBC, the
MultiValue BASIC dialect used in jBASE and Temenos T24.

- **Read the guide** at [jbc-lang.org](https://jbc-lang.org/). The
  [jbc-language repository](https://github.com/jbc-lang/jbc-language) contains
  the guide’s source, grammar, and function catalogue.
- **Try the compiler** with [jbcc](https://github.com/jbc-lang/jbcc), an
  MIT-licensed jBC-to-C compiler with runnable examples. Its grammar has
  been tested against T24 R07 and R10 sources, and runtime support is
  still in progress.

## jbcc is on PyPI

[jbcc 0.1.0](https://pypi.org/project/jbcc/) is available on PyPI. Run this
example from any directory with uv and a C99 compiler.

```sh
printf '%s\n' 'CRT "Hello, jBC!"' > hello.b
uvx jbcc --run hello.b
```
