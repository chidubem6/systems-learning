# 08 — Mini grep

## Goal
Build a Unix-style text search utility. This project combines file processing, command-line interfaces, buffers, and string searching into a useful systems tool.

## What you are building
Example:

```text
$ ./mygrep error server.log
42: connection error
88: fatal error while reading socket
```

Later extensions can support flags such as case-insensitive matching and recursive directory search.

## Required features
- Accept a search term and file path through command-line arguments.
- Read the file without loading the entire file unnecessarily.
- Print matching lines.
- Print useful errors for missing files or invalid arguments.
- Optionally print line numbers.

## Inputs
- Search pattern.
- One or more file paths.
- Optional command-line flags.

## Outputs
- Matching lines written to standard output.
- Diagnostics written for invalid input or file errors.
- Meaningful process exit status.

## Constraints
- Implement matching yourself for the base version.
- Process input incrementally using buffers.
- Keep command-line parsing separate from search logic.

## Concepts introduced
- practical `argc` / `argv`
- command-line option parsing
- buffered I/O
- standard output vs standard error
- exit codes
- directory traversal as an extension

## Concepts reinforced
- strings
- files
- arrays and buffers
- pointers
- modular program design

## Completion criteria
The tool can search real text files reliably, handles invalid usage cleanly, and you can explain how data moves from disk into your buffer and through the matching algorithm.
