# Systems Learning

A progressive project-based roadmap for learning C and systems programming by building increasingly lower-level software.

The purpose of this repository is not to complete tutorials. Each project is a specification that creates a reason to learn the next concept.

## Learning method

For each project:

1. Read the project README and understand the expected behaviour.
2. Define the smallest feature you can implement next.
3. Attempt it yourself.
4. When you hit a knowledge gap, identify the exact concept or API you do not understand.
5. Read documentation and build a tiny experiment if necessary.
6. Return to the project and implement the feature.
7. Be able to explain the code and the underlying mechanism before moving on.

Avoid searching for complete project solutions.

## Roadmap

| # | Project | Main new concepts |
|---|---|---|
| 01 | Number Toolkit | syntax, control flow, functions, basic arrays |
| 02 | Text Statistics | strings, characters, files, buffers |
| 03 | Dynamic Todo List | pointers, structs, dynamic memory |
| 04 | Persistent Contact Book | modules, headers, persistence |
| 05 | Dynamic Array | `void *`, pointer arithmetic, resizing |
| 06 | Linked List | linked structures, pointer-to-pointer |
| 07 | Hash Table | hashing, collisions, load factor |
| 08 | Mini grep | Unix-style CLI tools, buffered processing |
| 09 | Memory Allocator | memory layout, alignment, fragmentation |
| 10 | Unix Shell | processes, `fork`, `exec`, pipes, signals |
| 11 | HTTP Server | TCP sockets, HTTP, protocol parsing |
| 12 | Thread Pool Server | threads, mutexes, condition variables |
| 13 | Key-Value Store | storage engines, durability, recovery |
| 14 | Interpreter / VM | lexing, parsing, ASTs, runtime design |
| 15 | Capstone | architecture, profiling, integration |

## Recommended reference hierarchy

When stuck, prefer:

1. C language/library reference documentation.
2. Linux/POSIX manual pages for operating-system APIs.
3. Compiler diagnostics and GCC/Clang documentation.
4. Focused books/guides for deeper explanation.
5. AI/search only after you have identified the specific thing you do not understand.

The question to ask is not "How do I build this whole project?" It is "What do I need to understand well enough to implement the next piece?"

## Progress rule

Do not move to the next project merely because the current program runs. Move on when you can explain the core concepts the project was designed to teach and can debug ordinary failures without copying a full solution.
