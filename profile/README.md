# jBC Language

An unofficial reference guide and an experimental compiler for jBC, the
MultiValue BASIC dialect used in jBASE and Temenos T24. Its grammar has been tested
against the T24 R07, R10, R13 and R19 source corpora.

- **Read the guide** at [jbc-lang.org](https://jbc-lang.org/). The
  [jbc-language repository](https://github.com/jbc-lang/jbc-language) contains
  the guide’s source, grammar, and function catalogue.
- **Run jBC in your browser** with the [jBC Playground](https://online.jbc-lang.org/).
- **Try the native compiler** with [jbcc](https://github.com/jbc-lang/jbcc), an
  MIT-licensed jBC-to-C compiler with runnable examples. Runtime support
  is still in progress.

## jbcc is on PyPI

[jbcc 0.7.0](https://pypi.org/project/jbcc/0.7.0/) is available on PyPI. It
translates every Temenos program, subroutine and function in the T24 R07,
R10 and R13 corpora to C99, and 39,669 of the 39,675 units of the
componentised R19 corpus, with component calls checked against their
declarations. Run this example from any directory with uv and
a C99 compiler.

```sh
printf '%s\n' 'CRT "Hello, jBC!"' > hello.b
uvx jbcc --run hello.b
```
