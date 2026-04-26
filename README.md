# Project README

## Overview
This project is a C/C++ application that demonstrates the use of basic linear algebra operations, matrix transformations, and 3D vector calculations. It includes features such as:

- Basic matrix operations (creation, multiplication, inversion).
- Transformations like translation, rotation, scaling.
- 3D vector operations including addition, subtraction, dot product, cross product.

## Features
- Matrix creation and manipulation.
- Vector operations.
- Basic transformations in 3D space.

## Project Structure
```
<Project>/
├── build/              # .exe files produced by Main.c
├── bin/                # .so / .dll produced by *.c in libs
├── libs/               # *.c for bin
├── lib/                # librarys for my own languages
├── code/               # scripts from my custom languages for example .rex, .ll, .omml
├── data/               # Datafile for example .txt or dumped files
├── assets/             # images and sound files
├── src/                # source code
│   ├── Main.c          # Entry point
│   └── *.h             # stand alone Header-based C-files, without *.c files that implement it
├── Makefile.linux      # Linux Build configuration
├── Makefile.windows    # Windows Build configuration
├── Makefile.wine       # Wine Build configuration
└── README.md           # This file
└── LICENCE
└── .gitignore
```

## Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools

## Build & Run
### Linux
To build and run the project on Linux:

```sh
cd <Project>
make -f Makefile.linux all
./build/Main
```

### Windows
To build and run the project on Windows:

```sh
cd <Project>
make -f Makefile.windows all
./build/Main.exe
```

### Wine
To cross-compile and run the project on Linux for Windows:

```sh
cd <Project>
make -f Makefile.wine all
./build/Main.exe
```

These steps will compile the source code and execute the resulting executable in the `build` directory.