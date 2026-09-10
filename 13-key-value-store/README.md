# 13 — Persistent Key-Value Store

## Goal
Build a tiny persistent database that stores key-value pairs on disk. The aim is to understand storage-engine fundamentals: serialization, indexing, append-only persistence, compaction, and recovery.

## What you are building
Example interaction:

```text
db> SET name Chidubem
OK

db> GET name
Chidubem

db> DELETE name
OK
```

Data must still exist after the program is closed and restarted.

## Required features
- `SET key value`
- `GET key`
- `DELETE key`
- Persist writes to disk.
- Rebuild in-memory state after restart.
- Maintain an in-memory index for fast lookup.
- Handle malformed or incomplete input safely.

## Stretch features
- Append-only log.
- Compaction.
- Checksums.
- Binary record format.
- Crash recovery.

## Inputs
- Commands and key-value data from the terminal or a simple protocol.

## Outputs
- Retrieved values.
- `OK`, not-found, or error responses.
- Persistent storage file(s).

## Constraints
- Build persistence yourself using file APIs.
- Do not embed SQLite or another database.
- Document the on-disk format you choose.
- The system must have deterministic recovery behaviour.

## Concepts introduced
- storage engines
- serialization
- binary/text record formats
- append-only logs
- in-memory indexes
- durability
- recovery
- checksums
- compaction

## Concepts reinforced
- hash tables
- file I/O
- buffers
- structs
- memory ownership
- error handling

## Completion criteria
You can explain how a write becomes durable, how restart recovery works, how the index points to stored data, and what happens if the process stops unexpectedly during a write.
