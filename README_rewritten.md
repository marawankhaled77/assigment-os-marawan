# Process Management & Compilation Lab

[![Language](https://img.shields.io/badge/language-C-blue.svg)](https://en.wikipedia.org/wiki/C_%28programming_language%29)
[![OS](https://img.shields.io/badge/os-Linux-green.svg)](https://www.linux.org/)

## Overview

This repository contains C programs that demonstrate key Operating System concepts. The project includes examples of process creation, linking, loading, and automated compilation.

## Project Structure

```
assignment2_OS_marawan/
├── process_creation.c   # Demonstrates fork() behavior (by Marawan)
├── file1.c              # Linker example (part 1)
├── file2.c              # Linker example (part 2)
├── simple_program.c     # Loader demonstration
├── Makefile             # Build automation (by Marawan)
└── README.md
```

## Build Instructions

To compile and run the programs, use the following commands:

```bash
make all               # Compile all programs
make process_creation  # Compile process_creation.c
make output_program    # Compile linker demonstration
make simple_program    # Compile loader demonstration
make run               # Execute all compiled programs
make clean             # Remove build artifacts
```

## Implementation Details

### 1. Process Creation - `process_creation.c`

* Demonstrates how `fork()` creates a child process.
* Parent process continues execution; child receives a unique PID.
* Both processes run concurrently.
* Example written and documented by Marawan.

### 2. Linker Demonstration - `file1.c` + `file2.c`

* Shows how the linker resolves symbols and combines multiple compilation units into a single executable.

### 3. Loader Demonstration - `simple_program.c`

* Illustrates how executables are loaded into memory.
* Shows mapping of libraries and preparation for execution.

## Linker vs Loader

| Feature | Linker            | Loader             |
| ------- | ----------------- | ------------------ |
| Phase   | Compile-time      | Run-time           |
| Input   | Object files      | Executable         |
| Output  | Executable file   | Running process    |
| Task    | Symbol resolution | Load, map, and run |

## Environment

* GCC compiler
* Linux / POSIX OS
* C99 or later

## Author

Lab 5 Assignment - Operating Systems (by Marawan)

## License

MIT License (Educational Use)
