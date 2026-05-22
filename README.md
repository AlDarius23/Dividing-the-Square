# Dividing-the-Square

A 2D interactive logic game developed in C++ using the `graphics.h` (WinBGIm) library. The goal is to completely fill an 8x8 grid with colors, strictly following adjacency rules from the starting points.

## Features

- **Custom GUI:** Intuitive main menu, instructions window, and level selection screens.
- **Mouse-based Mechanics:** - Right-Click: Activate the color of an available circle.
  - Left-Click: Fill an adjacent cell with the active color.
- **Game Modes:**
  - **Random:** Procedurally generates random starting points on the grid.
  - **Custom:** Allows the player to create their own puzzle by manually adding/removing starting circles.
  - **Levels:** A campaign featuring 10 hardcoded levels with predefined architectures.

## Technologies

- **Language:** C++
- **Graphics:** WinBGIm (`graphics.h`)
- **System:** Windows API (for screen resolution detection and mouse input handling)

## How to Run

To compile and run this project, you need an environment configured to support `graphics.h` on modern systems:
1. Install **TDM-GCC 32-bit** (the app expects the compiler at `C:\TDM-GCC-32`).
2. Add the `libbgi.a` library to the `lib` folder and `graphics.h` / `winbgim.h` to the `include` folder of your compiler.
3. Add the following linker parameters:
   `-lbgi -lgdi32 -lcomdlg32 -luuid -loleaut32 -lole32`
4. Compile and run `main.cpp`.
