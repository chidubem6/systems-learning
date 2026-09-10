# 01 — Number Toolkit

## Goal
Build a small command-line program that performs several numerical operations. The purpose is not to create an impressive application; it is to become comfortable writing, compiling, running, and structuring basic C programs.

## What you are building
When the program starts, it should display a menu similar to:

```text
Number Toolkit

1. Check if a number is prime
2. Calculate factorial
3. Generate Fibonacci sequence
4. Calculate statistics for a set of numbers
5. Exit

Choose an option: 
```

The user chooses an option, provides the required input, and the program prints the result.

## Required features

### 1. Prime checker
Input:
```text
Enter a number: 17
```

Output:
```text
17 is prime.
```

### 2. Factorial calculator
Input:
```text
Enter a non-negative integer: 5
```

Output:
```text
5! = 120
```

### 3. Fibonacci generator
Input:
```text
How many numbers? 7
```

Output:
```text
0 1 1 2 3 5 8
```

### 4. Basic statistics
The program asks the user for several numbers and calculates at least:
- minimum
- maximum
- sum
- average

Example input:
```text
How many numbers? 5
Enter values: 10 4 8 2 6
```

Example output:
```text
Minimum: 2
Maximum: 10
Sum: 30
Average: 6.00
```

## Inputs
- menu selection
- integers or decimal values depending on the operation
- number of values to process

## Outputs
- numerical results printed to the terminal
- useful error messages for invalid input

## Constraints
- Keep the program terminal-based.
- Split each operation into its own function.
- Do not use dynamic memory yet.
- Do not try to over-engineer the project.

## Concepts this project should teach
- compiling and running C
- `main`
- variables and primitive types
- arithmetic operators
- `if` / `else`
- `switch`
- `for` and `while` loops
- functions
- function parameters and return values
- basic arrays
- terminal input/output with `printf`, `scanf`, or `fgets`
- basic input validation

## Completion criteria
You are finished when you can explain how every function works and the program can repeatedly accept menu choices until the user selects Exit.

## Learning rule
When you encounter something you do not understand, stop and learn only the concept required to move forward. Do not search for a complete implementation of the project.
