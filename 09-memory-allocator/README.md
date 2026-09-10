# 09 — Memory Allocator

## Goal
Build a simplified allocator to understand what `malloc`-style memory management has to do internally.

## What you are building
Expose functions conceptually similar to:

```text
my_malloc(size)
my_free(ptr)
```

Manage a fixed region of memory yourself and track which blocks are allocated or free.

## Required features
- Allocate blocks from a managed memory region.
- Store metadata for each block.
- Free previously allocated blocks.
- Reuse freed blocks.
- Split blocks when useful.
- Coalesce adjacent free blocks.

## Inputs
- Allocation sizes.
- Pointers previously returned by your allocator.

## Outputs
- Pointer to usable memory on successful allocation.
- `NULL` or equivalent failure when no suitable block exists.

## Constraints
- Do not call `malloc` to satisfy each user allocation.
- Manage a larger backing memory region yourself.
- Respect alignment requirements.
- Clearly separate allocator metadata from user memory.

## Concepts introduced
- raw memory layout
- alignment
- pointer arithmetic
- block headers
- free lists
- fragmentation
- block splitting and coalescing

## Concepts reinforced
- linked lists
- pointers
- structs
- ownership
- defensive programming

## Completion criteria
You can draw your allocator's memory layout, explain how an allocation is selected, how blocks are split/coalesced, and why fragmentation occurs.
