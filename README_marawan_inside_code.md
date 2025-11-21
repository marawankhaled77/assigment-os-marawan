# Process Management & Compilation Lab

[![Language](https://img.shields.io/badge/language-C-blue.svg)](https://en.wikipedia.org/wiki/C_(programming_language))
[![OS](https://img.shields.io/badge/os-Linux-green.svg)](https://www.linux.org/)

## Overview

This project showcases essential Operating System concepts through
practical C programs. It includes demonstrations of process creation,
linking, loading, and automated compilation.

## Project Structure

    assignment2_OS_marawan/
    ├── process_creation.c   # Demonstrates fork() behavior, created by marawan
    ├── file1.c              # Linker example (part 1)
    ├── file2.c              # Linker example (part 2)
    ├── simple_program.c     # Loader demonstration
    ├── Makefile             # Build automation (edited by marawan)
    └── README.md

## Build Instructions

``` bash
make all          # Compile all programs - marawan build
make process_creation
make output_program
make simple_program
make run          # Execute all programs
make clean        # Remove build artifacts
```

## Implementation Breakdown

### 1. Process Creation --- `process_creation.c`

Shows how `fork()` creates a child process: - Parent continues
execution. - Child receives a separate PID. - Both processes run
concurrently. - Example written and documented by marawan.

### 2. Linker Demonstration --- `file1.c` + `file2.c`

Demonstrates how the linker resolves symbols and combines compilation
units into one executable.

### 3. Loader Demonstration --- `simple_program.c`

Illustrates loading an executable into memory, mapping libraries, and
preparing execution.

## Linker vs Loader

  Feature   Linker              Loader
  --------- ------------------- --------------------
  Phase     Compile-time        Run-time
  Input     Object files        Executable
  Output    Executable file     Running process
  Task      Symbol resolution   Load, map, and run

## Environment

-   GCC compiler
-   Linux / POSIX OS
-   C99 or later

## Author

Operating Systems --- Lab 5 Assignment (by marawan)

## License

MIT License (Educational Use)
