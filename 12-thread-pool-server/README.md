# 12 — Thread Pool + Concurrent Server

## Goal
Extend the HTTP server so it can handle multiple clients concurrently using a fixed worker pool. This project introduces shared-memory concurrency and synchronization.

## What you are building
Conceptually:

```text
incoming connections
        |
        v
+------------------+
|   work queue     |
+------------------+
   |      |      |
   v      v      v
worker  worker  worker
```

The main thread accepts connections and places work into a queue. Worker threads remove connections from the queue and process them.

## Required features
- Create a fixed number of worker threads.
- Implement a shared work queue.
- Main thread accepts connections and enqueues them.
- Workers sleep when there is no work.
- Workers wake when work becomes available.
- Protect shared queue state correctly.
- Shut down workers cleanly.

## Inputs
- Incoming HTTP client connections.

## Outputs
- Concurrent HTTP responses.
- Server diagnostics for errors.

## Constraints
- Use threads directly rather than a concurrency framework.
- Avoid busy-waiting.
- Protect every shared mutable data structure appropriately.
- Be able to justify where locks are and are not required.

## Concepts introduced
- threads
- `pthread_create` / `pthread_join`
- mutexes
- condition variables
- critical sections
- race conditions
- deadlocks
- producer-consumer pattern
- work queues

## Concepts reinforced
- sockets
- linked queues or dynamic arrays
- pointers
- ownership
- resource cleanup

## Completion criteria
Multiple clients can be served concurrently, and you can explain what data is shared between threads, how each synchronization primitive protects it, and what race would occur if that protection were removed.
