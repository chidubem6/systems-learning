# 05 — Dynamic Array Library

## Goal
Build your own resizable array abstraction. This project moves you from using dynamic memory to designing a reusable memory-owning data structure.

## What you are building
A small library that supports operations conceptually similar to:

```text
create
push
get
set
remove
resize
destroy
```

The structure should track both its current length and its allocated capacity.

## Required features
- Create an empty dynamic array.
- Append elements.
- Read and update elements by index.
- Remove elements.
- Grow capacity when full.
- Free all owned memory.
- Detect invalid indexes.

## Inputs
- Elements supplied by a small test/demo program.
- Indexes and values passed into the library functions.

## Outputs
- Stored values returned to the caller.
- Success/failure information for invalid operations or failed allocations.

## Constraints
- Implement the storage yourself with `malloc` / `realloc` / `free`.
- Track `length` separately from `capacity`.
- Do not call an existing vector library.
- Prefer a generic design using `void *` once you understand the simpler typed version.

## Concepts introduced
- `void *`
- pointer arithmetic
- `size_t`
- memory copying
- `memcpy` / `memmove`
- capacity growth strategies
- generic data storage
- API design for a C library

## Concepts reinforced
- pointers
- structs
- allocation and reallocation
- ownership
- header/source separation

## Completion criteria
You can explain why dynamic arrays usually allocate more capacity than their current length, how resizing works, and how the library calculates the address of an arbitrary element.
