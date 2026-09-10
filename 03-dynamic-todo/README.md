# 03 — Dynamic Todo List

## Goal
Build a terminal todo application whose tasks are stored dynamically in memory. This project exists to force you to understand pointers, structs, allocation, resizing, and memory ownership.

## What you are building
Example interaction:
```text
Todo
1. Add task
2. List tasks
3. Complete task
4. Delete task
5. Exit
```

A task should have at least an ID, title, and completion state.

## Required features
- Add a task.
- List all tasks.
- Mark a task complete.
- Delete a task.
- Support a changing number of tasks at runtime.
- Release all allocated memory before exit.

## Inputs
- Menu choices
- Task titles
- Task IDs

## Outputs
- Task lists
- Confirmation messages
- Errors for invalid IDs or invalid input

## Constraints
- Store tasks using dynamically allocated memory.
- Represent a task with a `struct`.
- Do not use a fixed-size task array as the final implementation.
- Every successful allocation must have a clear owner and eventual `free`.

## Concepts introduced
- pointers
- address-of and dereference operators
- structs
- `typedef`
- `malloc`
- `calloc`
- `realloc`
- `free`
- `sizeof`
- pointer-to-struct syntax (`->`)
- memory ownership

## Concepts reinforced
- arrays
- functions
- strings
- loops
- input validation

## Completion criteria
You can explain where each allocated block comes from, who owns it, when it is resized, and when it is freed. The program can add and delete arbitrary numbers of tasks without leaking memory.
