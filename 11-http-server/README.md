# 11 — HTTP Server

## Goal
Build a small HTTP/1.1 server directly on top of TCP sockets. The purpose is to understand what web frameworks hide: listening sockets, connections, byte streams, protocol parsing, and response construction.

## What you are building
Start a server such as:

```text
$ ./server 8080
Listening on port 8080...
```

Then a client can send:

```http
GET /hello HTTP/1.1
Host: localhost
```

And receive:

```http
HTTP/1.1 200 OK
Content-Type: text/plain
Content-Length: 11

Hello world
```

## Required features
- Create a TCP socket.
- Bind it to a port.
- Listen for incoming connections.
- Accept clients.
- Read an HTTP request.
- Parse at least the request method and path.
- Return valid HTTP responses.
- Support at least `/` and `/hello` routes.
- Return `404 Not Found` for unknown routes.
- Close connections cleanly.

## Inputs
- TCP connections.
- Raw HTTP request bytes.

## Outputs
- Correctly formatted HTTP responses.
- Useful server-side diagnostics.

## Constraints
- Do not use an HTTP server library or web framework.
- Use the operating system socket API directly.
- Treat received data as bytes and do not assume one `recv` call always contains a complete request.

## Concepts introduced
- TCP sockets
- `socket`
- `bind`
- `listen`
- `accept`
- `recv`
- `send`
- network byte streams
- socket/file descriptors
- HTTP message structure
- protocol parsing

## Concepts reinforced
- buffers
- strings
- parsing
- pointers
- error handling
- operating-system APIs

## Completion criteria
A browser or `curl` can successfully talk to your server, and you can explain the path from TCP connection acceptance through HTTP parsing to response transmission.
