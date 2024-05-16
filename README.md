## Introduce

Welcome to our final DSA project. 

Our group has 3 people: Pham Phu Quoc, Chau Thanh Phat and Nguyen Thi Minh Chau.
We has decided to code Minesweeper game by Java for this project. 
The game mainly coded on Visual Studio Code and pushrd into Github, all the graphics 2D are designed using "Pixel art maker website" by our group members. Hope you will like it.

## Overview

I. Description

When you start the game, you will see a grid of cells on the screen. Each cell represents a hidden tile.

The game features a smiley face button, which serves as a reset button. You can click on it to start a new game or reset the current game.

To uncover a cell, you can left-click on it. If the clicked cell contains a mine, the game ends, and you lose. Otherwise, the cell will reveal a number indicating the number of mines in the adjacent cells.

If you suspect that a cell contains a mine, you can right-click on it to place a flag. This helps you mark cells that you think are mines and avoid accidentally clicking on them.

If you uncover all the cells that do not contain mines, you win the game.

The game also includes features like an undo button, which allows you to undo your moves, and a timer that keeps track of the time elapsed during the game.

The game provides visual feedback through different colors and symbols to indicate the state of the cells, such as revealed cells, flagged cells, and mines.

II. Main funtions

- Initialize Game: Sets up the initial state of the game, including the size of the board, number of mines, and positions of mines.

- Render Board: Displays the game board on the screen, showing the hidden cells and their corresponding numbers or mine symbols.

- Left-Click Action: Handles the action when a cell is left-clicked. It checks if the clicked cell contains a mine, reveals the number of adjacent mines, and recursively reveals neighboring cells if the clicked cell is empty.

- Right-Click Action: Handles the action when a cell is right-clicked. It toggles the flag on the cell to mark it as a potential mine.

- Smiley Button Action: Resets the game when the smiley face button is clicked. It generates a new board with randomized mine positions.

- Undo Action: Undoes the last move, allowing the player to revert their actions.

- Timer: Keeps track of the time elapsed during the game, providing a sense of urgency and challenge.

- Victory Check: Checks if the game is won by verifying if all non-mine cells are uncovered.

- Game Over: Handles the game over scenario when a mine is clicked. It reveals all the mine locations and ends the game.

- Mouse Movement: Tracks the mouse movement on the game board, highlighting cells under the cursor and providing visual feedback to the player.
  
## Abstraction

Here are the abstractions that we use in the game:

1. Entity: This abstraction represents the different entities or objects within the game, such as the Mine, Board, Flagger, Smiley, TimeCounter, Undo, and GameState. Each entity encapsulates its own functionality and behavior.

2. GUI: The GUI abstraction manages the graphical user interface of the game. It includes the GamePanel, which extends JPanel and handles the rendering and interaction logic of the game.

3. Control: The Control abstraction includes the control logic of the game. It consists of classes like GameFrame, which extends JFrame and serves as the main frame for the game. It also manages the initialization and setup of the game components.

4. MouseListener and MouseMotionListener: These interfaces represent abstractions for handling mouse events in the game. They are implemented by classes within the GamePanel to capture and respond to mouse movements and clicks.

5. Thread: The Thread abstraction is used to run the game loop and update the game state continuously. It ensures smooth rendering and responsiveness of the game by executing the game logic in a separate thread.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).
