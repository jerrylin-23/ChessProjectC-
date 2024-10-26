# Chess Project

A fully functional chess game with both text-based and graphical interfaces, supporting human and AI players. Developed for CS246 Spring 2024.
![image](https://github.com/user-attachments/assets/62c849cc-eeef-4748-9156-8d0b4972b33a)

## Features
- Dual display modes: Text-based and graphical (X11)
- Multiple player types: Human vs Human, Human vs AI, or AI vs AI
- Four AI difficulty levels
- Complete chess rules including castling, en passant, and pawn promotion
- Game state saving and loading
- Setup mode for custom board configurations

## Installation

### Prerequisites
- X11 library for graphical display
- C++ compiler

### Compilation
```bash
make
```

### Running the Game
```bash
./chess
```

## Game Commands

### Basic Commands
- `game white-player black-player` - Start new game (e.g., `game human computer1`)
- `move e2 e4` - Move piece from e2 to e4
- `resign` - Concede game
- `setup` - Enter setup mode
- `save` - Save current game state to board.txt

### Setup Mode
- `+ K e1` - Place white king on e1
- `- e1` - Remove piece from e1
- `= color` - Set turn
- `done` - Exit setup mode

## Project Structure

### Core Components
- Board and game logic (`board.cc`)
- Player management (`player.cc`, `human.cc`, `ai.cc`)
- Display systems (`textDisplay.cc`, `graphicsDisplay.cc`)
- Game control (`controller.cc`)

### Chess Pieces
- Individual piece implementations for King, Queen, Bishop, Knight, Rook, and Pawn
- Base piece class with common functionality

## Authors
- jy3lin
- pvajpeyi
- adhuka

For source code access, contact: jy3lin@uwaterloo.ca
