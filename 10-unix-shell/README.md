# 10 — Unix Shell

## Goal
Build a small command shell to understand how Unix launches programs and connects processes together.

## What you are building
Example:

```text
myshell> ls -la
myshell> echo hello
myshell> cat file.txt | grep error
myshell> exit
```

## Required features
- Display a prompt.
- Read a command from the user.
- Parse the command and arguments.
- Launch external programs.
- Wait for child processes.
- Support an `exit` built-in.
- Support at least one pipe between two commands.
- Handle Ctrl+C sensibly.

## Inputs
- Shell commands entered interactively.

## Outputs
- Output from launched programs.
- Shell errors for malformed or unavailable commands.

## Constraints
- Use operating-system process APIs rather than invoking another shell to execute commands.
- Keep parsing, execution, and built-in command handling separated.

## Concepts introduced
- processes
- `fork`
- `exec`
- `wait`
- pipes
- file descriptors
- `dup2`
- signals
- environment and `PATH`

## Concepts reinforced
- parsing
- strings
- dynamic memory
- arrays
- error handling

## Completion criteria
You can explain exactly what happens from the moment the user presses Enter to the point where a child program executes, exits, and control returns to your shell.
