# ASCII Donut

This program renders a spinning 3D donut shape using ASCII characters in your terminal.

## Description

The code implements the mathematical formulas to project a 3D torus (donut shape) onto a 2D terminal screen. It then "illuminates" the surface based on a light source and maps different brightness levels to a set of ASCII characters. The animation is achieved by rotating the donut in successive frames.

## Original Author and Source

This version of the ASCII donut program is based on the work of **Andy Sloane**. He originally wrote the C code in 2006 and later published a detailed explanation of the mathematics involved.

You can find his explanation and the original code here:
[Donut math: how donut.c works](https://www.a1k0n.net/2011/07/20/donut-math.html)

This repository contains a deobfuscated version of that code.

## How to Compile and Run

This program is written in C. You'll need a C compiler (like GCC) and the math library to build it.

1.  **Compile the code:**
    Open your terminal and run the following command:
    ```bash
    gcc -o donut donut_deobfuscated -lm
    ```
    (The file containing the source code in this repository is named `donut_deobfuscated`)

2.  **Run the program:**
    ```bash
    ./donut
    ```

You should see a spinning ASCII donut in your terminal! Press `Ctrl+C` to exit.

## Requirements

*   A C compiler (e.g., GCC)
*   The standard C library
*   The math library (`libm`)

The code uses functions like `printf`, `memset`, `sin`, `cos`, and `usleep` (or a similar delay function). These are generally available on most Unix-like systems (Linux, macOS). The original obfuscated version sometimes included `conio.h` which is common in older DOS/Windows environments, but this deobfuscated version should be fairly portable.

## Enjoy the spin!
