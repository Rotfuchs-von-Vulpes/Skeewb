> ## A minimalist, modular voxel game/engine with focus on flexibility and performance 

# Modules

The whole engine is split into different, swappable modules, which are libraries (.dll/.so) loaded at runtime by the core executable.

Each [[Module]] can communicate with other modules by the core config/resource system and interfaces.
# Compiling

## Prerequisites
- C compiler: gcc/clang/mingw-w64
- Cmake
- SDL required libraries (Linux)

## Linux (gcc/clang) / Windows (MinGW)
```bash
gcc crane.c -o crane # clang works too 
./crane              # may be .exe in Windows
```

# Creating a module

An example module can be created using the following commands:
```bash
./crane example
cd examplemod
gcc crane.c -o crane # examplemod's own crane
./crane
```

Check [[Getting Started]] for more information.