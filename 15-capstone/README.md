# 15 — Capstone Systems Project

## Goal
Use the skills from the previous projects to design and build one substantial systems project without following a step-by-step tutorial.

## Choose one direction
Examples:

- Redis-like in-memory server with persistence
- Git-like version control system
- small database engine
- BitTorrent client
- tiny container/runtime experiment

Do not choose based on what sounds most impressive. Choose a project whose internals you genuinely want to understand.

## What you are building
You define the exact product and protocol before implementation. Your specification should include:

- problem being solved
- supported operations
- inputs and outputs
- architecture
- core data structures
- persistence/networking model if relevant
- error behaviour
- performance goals
- explicit non-goals

## Required properties
Whatever you choose, the project should combine several prior areas rather than introducing only one isolated concept. It should require at least four of the following:

- manual memory management
- custom data structures
- file/storage management
- operating-system APIs
- networking
- concurrency
- parsing/protocol design
- performance measurement

## Inputs
Defined by the selected project. Examples include commands, files, network packets, or protocol messages.

## Outputs
Defined by the selected project. Examples include persisted data, network responses, generated files, or command output.

## Constraints
- Do not start from a full tutorial implementation.
- Write a design/specification before substantial coding.
- Break implementation into small vertical slices.
- Add tests for important invariants.
- Use debugging and profiling tools where appropriate.
- Document major design decisions and trade-offs.

## Concepts introduced
- larger-system architecture
- performance profiling
- requirements decomposition
- engineering trade-offs
- debugging complex systems
- integration of multiple systems concepts

## Concepts reinforced
Everything required by the chosen project.

## Completion criteria
The project has a defined specification, works end-to-end, has meaningful tests, and you can defend its architecture and implementation decisions without relying on memorised explanations.
