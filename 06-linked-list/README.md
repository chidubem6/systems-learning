# 06 — Linked List Library

## Goal
Build a reusable singly linked list and become comfortable manipulating relationships through pointers.

## What you are building
A small library supporting operations such as:

```text
insert_front
insert_back
find
remove
reverse
destroy
```

## Required features
- Create an empty list.
- Insert at the front and back.
- Find an element.
- Remove an element.
- Reverse the list.
- Destroy the entire list safely.

## Inputs
- Values passed by a demo/test program.
- Search values or predicates.

## Outputs
- Retrieved elements.
- Updated list structure.
- Success/failure information.

## Constraints
- Allocate each node dynamically.
- Do not represent the list internally as an array.
- Correctly update the head when operations affect the first node.

## Concepts introduced
- self-referential structs
- pointer-to-pointer patterns
- linked memory structures
- traversal
- insertion/removal without shifting arrays

## Concepts reinforced
- pointers
- dynamic memory
- ownership
- structs
- library APIs

## Completion criteria
You can draw the list on paper with addresses/pointers, explain why some operations require modifying the caller's head pointer, and safely free every node.
