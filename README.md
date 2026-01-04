# Monkey Parser
Monkey-Parser is an interpreter built for the "Monkey" programming language.

This project is based off the book, "Writing an Interpreter in Go" - Thorsten Ball.


## Monkey features
- C-like syntax
- variable bindings
- integers and booleans
- arithmetic expressions
- built-in functions
- first-class and higher-order functions
- closures
- a string data structure
- an array data structure
- a hash data structure

## Component of the interpreter
- Lexer
- Parser
- Abstract Syntax Tree (AST)
- Internal Object System
- Evaluator

---

## Lexical Analysis
Lexical Analysis (lexing) is the transformation of source code to tokens, done by a lexer/tokenizer/scanner. Tokens are small, categorizable data structures that get fed to the parser, which does another transformation and turns them into an AST.

```
Example: "let x = 5 + 5;"

Output:
[
    LET,
    IDENTIFIER("x"),
    EQUAL_SIGN,
    INTEGER(5),
    PLUS_SIGN,
    INTEGER(5),
    SEMICOLON
]
```