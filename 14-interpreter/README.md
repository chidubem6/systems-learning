# 14 — Interpreter / Virtual Machine

## Goal
Build a small programming language interpreter, then optionally evolve it into a bytecode virtual machine. This project combines parsing, recursive data structures, memory management, and runtime design.

## What you are building
A tiny language such as:

```text
let x = 10;
let y = x * 2;
print(y);
```

The implementation pipeline should conceptually become:

```text
source
  -> lexer
  -> tokens
  -> parser
  -> AST
  -> evaluator
```

A later extension may compile the AST into bytecode executed by a VM.

## Required features
- Tokenize source code.
- Parse expressions.
- Support numeric literals and arithmetic.
- Support variables.
- Support a `print` statement or equivalent.
- Build an AST rather than directly evaluating raw text.
- Produce useful syntax errors.

## Stretch features
- Boolean values.
- `if` statements.
- Loops.
- Functions.
- Lexical scope.
- Bytecode compiler.
- Stack-based virtual machine.

## Inputs
- Source code from a file or REPL.

## Outputs
- Program output.
- Lexer/parser/runtime errors with useful context.

## Constraints
- Write the lexer and parser yourself.
- Clearly separate lexing, parsing, and evaluation.
- Correctly free dynamically allocated syntax/runtime data.

## Concepts introduced
- lexical analysis
- tokens
- recursive-descent parsing
- grammars
- abstract syntax trees
- enums and unions
- recursive structures
- symbol tables
- environments and scope
- virtual machines as an extension

## Concepts reinforced
- pointers
- memory ownership
- hash tables
- dynamic arrays
- linked/recursive structures
- modular architecture

## Completion criteria
You can trace a statement from source characters to tokens, AST nodes, and runtime evaluation, and explain how variables are represented and resolved.
