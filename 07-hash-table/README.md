# 07 — Hash Table

## Goal
Build a key-value hash table from scratch. This project introduces hashing, collision handling, resizing, and average-case constant-time lookup.

## What you are building
A structure that supports operations such as:

```text
set("name", "Chidubem")
get("name")
delete("name")
```

## Required features
- Insert key-value pairs.
- Retrieve values by key.
- Update an existing key.
- Delete keys.
- Handle hash collisions correctly.
- Resize when the load factor becomes too high.

## Inputs
- Keys and values supplied by a demo/test program.

## Outputs
- Retrieved values.
- Success/failure information.

## Constraints
- Write your own hash function or implement a documented simple one.
- Do not use an existing hash-map implementation.
- Choose and document a collision strategy such as separate chaining.

## Concepts introduced
- hash functions
- buckets
- collisions
- load factor
- resizing and rehashing
- function pointers if you make hashing/comparison configurable

## Concepts reinforced
- dynamic arrays
- linked lists
- pointers
- ownership
- structs

## Completion criteria
You can explain how a key becomes a bucket index, why collisions are unavoidable, how your collision strategy works, and why resizing preserves correct lookup behaviour.
