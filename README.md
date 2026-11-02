# Minesweeper (C Language)

A classic Minesweeper game built from scratch using clean C architecture. This project showcases modular programming, memory management, file I/O operations, and algorithmic logic for grid generation and mine placement.

## Tech Stack & Concepts
- **Language:** C (C11 standard)
- **Build System:** GNU Make (Makefile)
- **Core Concepts:** Custom data structures, dynamic arrays, pointer manipulation, file parsing, multi-file source separation (`.h` / `.c`).

## Team & Collaboration (Academic Project)
This project was developed in a two-person team for a first-year subject of Computer Science course. 
- **My Contributions:**
  - Codesigned the core game logic engine and state management in `minelib.c`.
  - Implemented the custom game configuration loader (file I/O parsing from `game.txt`).
  - Authored the automated multi-file compilation system (`Makefile`).
- **Teammate's Contributions:**
  - Codesigned the core game logic engine and state management in `minelib.c`.
  - Developed the text-based UI/rendering layer in `main.c` and user input handling.

## Features
- **Custom Game Configuration:** The game dynamically reads grid dimensions and mine density from an external configuration file (`game.txt`).
- **Modular Design:** Complete decoupling of core game algorithms (`minelib`) from the input/output loop (`main`).
- **Memory Efficient:** Strict adherence to proper allocation and cleanup guidelines to avoid memory leaks.

## Project Structure
- `main.c` - Entry point, main game loop, and console UI rendering.
- `minelib.c` / `minelib.h` - Core game engine (grid initialization, reveal logic, mine validation).
- `game.txt` - Configuration file defining board matrix size and game variables.
- `Makefile` - Automated build automation script.

## How to Run Locally

### Prerequisites
Make sure you have GCC compiler and GNU Make installed on your system.

### Compilation
Open your terminal in the project root directory and run:
```bash
make
```
This will compile the source files and generate an executable binary.

### Running the Game
To start the game, execute the following command:
```bash
./minesweeper
```
*(Note: Ensure `game.txt` is present in the same directory as it is required to initialize the board).*

### Cleanup
To remove compiled object files and binaries:
```bash
make clean
```
