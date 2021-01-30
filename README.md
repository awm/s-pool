# S-Pool

_A shared memory, pool-based allocator with features for zero-copy buffer manipulation._

## Features

_TBD_

## Build

S-Pool is built as a static or shared library which may then be linked into your own application.

## Dependencies

_TBD_

## Instructions

The basic steps to build for the current host platform are as follows.  For more detailed
instructions, see the _[full documentation]_.

 1. Create a build directory:
    ```bash
    mkdir build
    cd build
    ```
 2. Generate the build files:
    ```bash
    cmake -G Ninja ..
    ```
 3. Build the library:
    ```bash
    ninja
    ```
The finished libraries will be located in `build/source`.

## License

**Copyright 2021 Andrew MacIsaac.**

Licensed under the terms of the [MPL-2.0](LICENSE.txt).
