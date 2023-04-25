# CLI Debugger

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
