<p align="center">
  <img src="https://raw.github.com/pest-parser/pest/master/pest-logo.svg?sanitize=true" width="80%"/>
</p>

# Awesome pest. The Elegant Parser [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome projects and tools using or for the pest parser generator in Rust


## Contents

pest is a general purpose parser written in Rust with a focus on accessibility,
correctness, and performance. It uses parsing expression grammars
(or [PEG]) as input, which are similar in spirit to regular expressions, but
which offer the enhanced expressivity needed to parse complex languages.

[PEG]: https://en.wikipedia.org/wiki/Parsing_expression_grammar


The recommended way to start parsing with pest is to read the official [book].

Other helpful resources:

* API reference on [docs.rs]
* play with grammars and share them on our [fiddle]
* find previous common questions answered or ask questions on [GitHub Discussions]
* leave feedback, ask questions, or greet us on [Gitter] or [Discord]

[book]: https://pest.rs/book
[docs.rs]: https://docs.rs/pest
[fiddle]: https://pest.rs/#editor
[Gitter]: https://gitter.im/pest-parser/pest
[Discord]: https://discord.gg/XEGACtWpT2
[GitHub Discussions]: https://github.com/pest-parser/pest/discussions

### Awesome lists

- [Projects using pest](#projects)
- [Tooling for pest](#tooling)


## Projects

Here are some example projects using pest:

- [pest_meta](https://github.com/pest-parser/pest/blob/master/meta/src/grammar.pest) (bootstrapped)
- [AshPaper](https://github.com/shnewto/ashpaper)
- [brain](https://github.com/brain-lang/brain)
- [cicada](https://github.com/mitnk/cicada)
- [comrak](https://github.com/kivikakk/comrak)
- [elastic-rs](https://github.com/cch123/elastic-rs)
- [graphql-parser](https://github.com/Keats/graphql-parser)
- [handlebars-rust](https://github.com/sunng87/handlebars-rust)
- [hexdino](https://github.com/Luz/hexdino)
- [Huia](https://gitlab.com/jimsy/huia/)
- [insta](https://github.com/mitsuhiko/insta)
- [jql](https://github.com/yamafaktory/jql)
- [json5-rs](https://github.com/callum-oakley/json5-rs)
- [mt940](https://github.com/svenstaro/mt940-rs)
- [Myoxine](https://github.com/d3bate/myoxine)
- [py_literal](https://github.com/jturner314/py_literal)
- [rouler](https://github.com/jarcane/rouler)
- [RuSh](https://github.com/lwandrebeck/RuSh)
- [rs_pbrt](https://github.com/wahn/rs_pbrt)
- [stache](https://github.com/dgraham/stache)
- [tera](https://github.com/Keats/tera)
- [ui_gen](https://github.com/emoon/ui_gen)
- [ukhasnet-parser](https://github.com/adamgreig/ukhasnet-parser)
- [ZoKrates](https://github.com/ZoKrates/ZoKrates)
- [Vector](https://github.com/timberio/vector)
- [AutoCorrect](https://github.com/huacnlee/autocorrect)
- [yaml-peg](https://github.com/aofdev/yaml-peg)
- [qubit](https://github.com/abhimanyu003/qubit)
- [caith](https://github.com/Geobert/caith) (a dice roller crate)
- [Melody](https://github.com/yoav-lavi/melody)

## Tooling

### IDE Support

- [pest IDE tools](https://github.com/pest-parser/pest-ide-tools) (a main repository with LSP server and VSCode extension)
- [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=pest.pest-ide-tools)
- [IntelliJ IDEA Plugin](https://plugins.jetbrains.com/plugin/12046-pest)
- [pest.vim](https://github.com/pest-parser/pest.vim)
- [pest-fmt](https://github.com/pest-parser/pest-fmt) can help to format
pest grammars (try it [online](https://pest.rs/#editor))
- [pest web debugger](https://github.com/tomtau/pest-web-debug)  (try it [online](http://tomtau.github.io/pest-web-debug/))

### Boilerplate reduction and testing

- [pest-ast](https://github.com/pest-parser/ast) can help to reduce boilerplate
when converting pest parse trees to abstract syntax trees
- [pest_consume](https://crates.io/crates/pest_consume) crate can 
help with the parse tree traversing boilerplate
- [pest-test](https://crates.io/crates/pest-test) is a testing framework for pest grammars


### CLI Debugger

There is a simple interactive command line debugger for pest grammars. It can be installed with:

```sh
cargo install pest_debugger
```

You can then run the interactive debugger by calling `pest_debugger` and view its help by typing `h` in its prompt:

```
> h

Use the following commands:
g <grammar filename>          - load .pest grammar
i <input filename>            - load input from a file
id <input text>               - load input directly from a single-line input
ba                            - add breakpoints at all rules
b <rule>                      - add a breakpoint at a rule
d <rule>                      - delete a breakpoint at a rule
da                            - delete all breakpoints
r <rule>                      - run a rule
c                             - continue
l                             - list breakpoints
h                             - help
```

The commands are self-explanatory; for a quick reference, the basic usage is:
```
> g ...file path to your grammar...
> i ...file path to your input...
> b ...name of the rule you want to stop at...
> r ...the rule to start running at...
```

:bulb: There is a tab completion for file paths and command history.

And then, once the debugger hits a breakpoint, you can continue the execution by typing:
```
> c
```

:bulb: You can also start up the debugger with command-line arguments that will do those steps during initialisation:

```sh
Usage: pest_debugger [options]

Options:
-g, --grammar <grammar file>    - load .pest grammar
-i, --input <input file>        - load input file
-r, --rule <rule>               - run rule
-b, --breakpoint <rule>         - breakpoint at rule
-s, --session <session file>    - load session history file
-h, --help                      - print this help menu
```


## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
