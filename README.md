# The T# Programming Language

Written with ANTLRv4 generated lexer/parser and C++. Now open source!

## Disclaimer

Not finished. Complete rewrite being done in C++, instead of Go.

## Build the thing, idiot

**You need the following, you need it:**
- ANTLRv4 AND the ANTLRv4 C++ Runtime - can be installed via Homebrew if you are on a Mac
- C++ Compiler (`clang++`/`g++` or whatever you use)

Once everything is up and running do the following commands in order, again you need ANTLRv4, with the C++ runtime and C++ running, you need it.

1. `antlr4 -Dlanguage=Cpp -listener -visitor -o gen TSharpLexer.g4 TSharpParser.g4`
2. `make`

Then run a `.tsharp` file:

`./tsharp your_file_name_here.tsharp`

Please note: Language is barely functional yet - was working OK on the prev. Go version, but C++ has `public`and `nullptr`, enough said.