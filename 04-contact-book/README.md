# 04 — Persistent Contact Book

## Goal
Build a contact manager that persists data between program runs. This project introduces multi-file C programs and persistent storage.

## What you are building
Example commands:
```text
contact add
contact list
contact find Alice
contact delete 42
```

Each contact should contain at least an ID, name, and one contact field such as phone number or email.

## Required features
- Add contacts.
- List contacts.
- Search contacts by name or ID.
- Delete contacts.
- Save contacts to disk.
- Reload saved contacts when the program starts again.

## Inputs
- Commands or menu selections
- Names
- Contact details
- IDs or search terms

## Outputs
- Contact records
- Search results
- Confirmation/error messages

## Constraints
- Split the project across multiple `.c` and `.h` files.
- Separate contact logic from persistence logic.
- Data must survive process termination.
- Handle missing or unreadable storage files gracefully.

## Concepts introduced
- header files
- declarations vs definitions
- separate compilation
- `#include`
- internal helper functions with `static`
- `FILE *`
- `fopen` / `fclose`
- text or binary persistence
- serialization basics

## Concepts reinforced
- pointers
- structs
- dynamic memory
- strings
- error handling

## Completion criteria
You understand how source files, header files, and compilation units work together, and contacts created in one program run are available after restarting the program.
