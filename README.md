**Chess Project**

**Overview**
This project implements a fully functional chess game with both text-based and graphical user interfaces. The game accommodates human and computer players, allowing for different levels of AI difficulty. The project was developed as part of the CS246 Spring 2024 course.
![image](https://github.com/user-attachments/assets/62c849cc-eeef-4748-9156-8d0b4972b33a)

To see the source code, please email me @ jy3lin@uwaterloo.ca

**Features**
Text-based and Graphical Display: The chess board can be displayed in both text format and a graphical interface using X11.
Human and Computer Players: Supports games between two human players, a human and a computer, or two computer players.
AI Difficulty Levels: Four levels of AI difficulty, from random moves to more sophisticated strategies.
Standard Chess Rules: Implements all standard chess rules including castling, en passant, pawn promotion, and check/checkmate detection.
Command Interpreter: A robust command interpreter that allows users to start games, make moves, and enter setup mode and save on going games.
File Descriptions

**Source Files**
**ai.cc:** 
    Implementation of the AI player 

**bishop.cc:** 
    Implementation of the Bishop piece and its valid moves.

**board.cc:** 
    Core logic for the chess board, including piece setup, move validation, and game state checks.

**controller.cc:** 
    Manages the game flow, player interactions, and updates to the board state.

**graphicsDisplay.cc:** 
    Handles the graphical representation of the chess board.

**human.cc:** 
    Implementation of the human player.

**king.cc:** 
    Implementation of the King piece and its valid moves.

**knight.cc:** 
    Implementation of the Knight piece and its valid moves.

**level_1.cc, level_2.cc, level_3.cc, level_4.cc:** 
    Implementations of AI strategies for different levels.

**main.cc:** 
    Entry point of the application, handling initialization and command processing.

**move.cc:** 
    Defines the Move structure used for representing piece movements.

**pawn.cc:** 
    Implementation of the Pawn piece and its valid moves.

**piece.cc:** 
    Base class for all chess pieces.

**player.cc:** 
    Base class for all players, human and AI.

**queen.cc:** 
    Implementation of the Queen piece and its valid moves.

**rook.cc:**
    Implementation of the Rook piece and its valid moves.

**square.cc:** 
    Represents a square on the chess board with x,y;

**textDisplay.cc:** 
    Handles the text-based representation of the chess board.

**view.cc:** 
    Abstract base class for the different views (text and graphical).

**Xwindow.cc:** 
    Manages the X11 window for graphical display.


**Header Files**
**ai.h:** Header for the AI player.
**bishop.h:** Header for the Bishop piece.
**board.h:** Header for the Board class.
**controller.h:** Header for the Controller class.
**graphicsDisplay.h:** Header for the GraphicsDisplay class.
**human.h:** Header for the Human player.
**king.h:** Header for the King piece.
**knight.h:** Header for the Knight piece.
**level_1.h, level_2.h, level_3.h, level_4.h:** Headers for different AI levels.
**move.h:** Header for the Move structure.
**pawn.h:** Header for the Pawn piece.
**piece.h:** Header for the Piece base class.
**player.h:** Header for the Player base class.
**queen.h:** Header for the Queen piece.
**rook.h:** Header for the Rook piece.
**square.h:** Header for the Square class.
**textDisplay.h:** Header for the TextDisplay class.
**view.h:** Header for the View base class.
**Xwindow.h:** Header for the Xwindow class.
**Compilation**

**To compile the project, ensure you have the necessary libraries for graphical display (X11). Use the following command to compile all source files:**

make

**To start the game, run the compiled executable:**

./chess

**Commands**
**game white-player black-player:**
     Starts a new game with specified players (e.g., game human computer[1-4]).
**move e2 e4:** 
    Moves a piece from e2 to e4.
**resign:** 
    Concedes the game.
**setup:** 
    Enters setup mode to manually configure the board.
**save:** 
    Prints current Board state onto a board.txt file so it can be loaded later

**Setup Mode Commands**
+ K e1: Places the white king on e1.
- e1: Removes the piece from e1.
= color: Sets the turn to the specified color.
done: Exits setup mode.

**Project Structure**
    Refer to the UML diagram (Chess Final Project UML.pdf) and project assignment (chessassignment.pdf) for detailed descriptions of the project structure and requirements.

**Notes**
Ensure your environment supports X11 for graphical display.


**Authors**
 jy3lin, pvajpeyi, adhuka 
