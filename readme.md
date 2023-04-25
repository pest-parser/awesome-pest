<p align="center">
  <img src="https://raw.github.com/pest-parser/pest/master/pest-logo.svg?sanitize=true" width="80%"/>
</p>

# Awesome Pest. The Elegant Parser [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome projects and tools using or for the pest parser generator in Rust


## Contents

pest is a general purpose parser written in Rust with a focus on accessibility,
correctness, and performance. It uses parsing expression grammars
(or [PEG](https://en.wikipedia.org/wiki/Parsing_expression_grammar)) as input, which are similar in spirit to regular expressions, but
which offer the enhanced expressivity needed to parse complex languages.

### Awesome lists

* [Resources](https://github.com/pest-parser/awesome-pest/blob/main/readme.md#resources)
* [Projects](https://github.com/pest-parser/awesome-pest/blob/main/readme.md#projects)
* [Tooling](https://github.com/pest-parser/awesome-pest/blob/main/readme.md#tooling)

## Resources

* [Book](https://pest.rs/book) - the recommended way to start parsing with pest is to read this official book.
* [API reference on docs.rs](https://docs.rs/pest)
* [fiddle editor on pest.rs](https://pest.rs/#editor) - play with grammars and share them on the official website.
* [Gitter](https://gitter.im/pest-parser/pest)
* [Discord](https://discord.gg/XEGACtWpT2)
* [GitHub Discussions](https://github.com/pest-parser/pest/discussions)

## Projects

Here are some example projects using pest:

* [pest_meta](https://github.com/pest-parser/pest/blob/master/meta/src/grammar.pest) (bootstrapped)
* [AshPaper](https://github.com/shnewto/ashpaper)
* [brain](https://github.com/brain-lang/brain)
* [cicada](https://github.com/mitnk/cicada)
* [comrak](https://github.com/kivikakk/comrak)
* [elastic-rs](https://github.com/cch123/elastic-rs)
* [graphql-parser](https://github.com/Keats/graphql-parser)
* [handlebars-rust](https://github.com/sunng87/handlebars-rust)
* [hexdino](https://github.com/Luz/hexdino)
* [Huia](https://gitlab.com/jimsy/huia/)
* [insta](https://github.com/mitsuhiko/insta)
* [jql](https://github.com/yamafaktory/jql)
* [json5-rs](https://github.com/callum-oakley/json5-rs)
* [mt940](https://github.com/svenstaro/mt940-rs)
* [Myoxine](https://github.com/d3bate/myoxine)
* [py_literal](https://github.com/jturner314/py_literal)
* [rouler](https://github.com/jarcane/rouler)
* [RuSh](https://github.com/lwandrebeck/RuSh)
* [rs_pbrt](https://github.com/wahn/rs_pbrt)
* [stache](https://github.com/dgraham/stache)
* [tera](https://github.com/Keats/tera)
* [ui_gen](https://github.com/emoon/ui_gen)
* [ukhasnet-parser](https://github.com/adamgreig/ukhasnet-parser)
* [ZoKrates](https://github.com/ZoKrates/ZoKrates)
* [Vector](https://github.com/timberio/vector)
* [AutoCorrect](https://github.com/huacnlee/autocorrect)
* [yaml-peg](https://github.com/aofdev/yaml-peg)
* [qubit](https://github.com/abhimanyu003/qubit)
* [caith](https://github.com/Geobert/caith) - a dice roller crate.
* [Melody](https://github.com/yoav-lavi/melody)

## Tooling

### IDE Support

* [pest IDE tools](https://github.com/pest-parser/pest-ide-tools) - a main repository with LSP server and VSCode extension.
* [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=pest.pest-ide-tools)
* [IntelliJ IDEA Plugin](https://plugins.jetbrains.com/plugin/12046-pest)
* [pest.vim](https://github.com/pest-parser/pest.vim)
* [pest-fmt](https://github.com/pest-parser/pest-fmt) - it can help to format
pest grammars (try it [online](https://pest.rs/#editor)).
* [pest web debugger](https://github.com/tomtau/pest-web-debug) - try it [online](http://tomtau.github.io/pest-web-debug/).

### Boilerplate reduction and testing

* [pest-ast](https://github.com/pest-parser/ast) - it can help to reduce boilerplate
when converting pest parse trees to abstract syntax trees.
* [pest_consume](https://crates.io/crates/pest_consume) - this crate can 
help with the parse tree traversing boilerplate.
* [pest-test](https://crates.io/crates/pest-test) - it is a testing framework for pest grammars.


### CLI Debugger

* [pest_debugger](https://docs.rs/pest_debugger/latest/pest_debugger/) - it is a crate for debugging pest grammars. It can be used as a CLI tool or as a library. [See instructions for using the CLI debugger](./debugger.md).

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
