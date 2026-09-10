# 02 — Text Statistics

## Goal
Build a command-line program that reads text and reports useful statistics. This project introduces C strings, character arrays, file reading, and character-by-character processing.

## What you are building
The program should accept either text input or a file and calculate statistics such as characters, words, lines, and longest word.

Example:
```text
$ ./textstats article.txt
Characters: 18294
Words: 3129
Lines: 274
Longest word: architecture
```

## Required features
- Count total characters.
- Count words separated by whitespace.
- Count lines.
- Find the longest word.
- Handle an empty file without crashing.

## Inputs
- A text file path supplied on the command line, or terminal text if you choose to support both.

## Outputs
- Character count
- Word count
- Line count
- Longest word
- Clear error if the file cannot be opened

## Constraints
- Process the text yourself rather than using a third-party library.
- Avoid dynamic memory unless you genuinely need it.
- Work character-by-character or buffer-by-buffer.

## Concepts introduced
- arrays
- C strings
- null terminators
- `char`
- character classification
- `argc` and `argv`
- file I/O
- EOF
- buffers

## Concepts reinforced
- loops
- conditionals
- functions
- input validation

## Completion criteria
You can explain what a C string actually is in memory, correctly process normal and empty files, and understand how your program detects word and line boundaries.
