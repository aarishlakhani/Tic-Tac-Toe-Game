Tic-Tac-Toe Game: README

Overview

This project is a simple implementation of a Tic-Tac-Toe game using JavaScript. The game alternates turns between two players, "X" and "O", and allows players to interact with the game board by clicking buttons. The game ends when all cells are filled, and a "Game Over" message is displayed.

Features

Dynamic Game Board Creation
The createGameBoard function programmatically creates the buttons for the game board.
Turn-Based Gameplay
The nextPlayer variable alternates between 'X' and 'O' to indicate the current player's turn.
Event Listeners
Each button on the board has a takeCell event listener to handle click events.
Game Over Detection
The isGameOver function determines if all buttons are disabled, signaling the end of the game.
Game Over Message
A message is displayed when the game is over using a label with the ID game-over-lbl.
How It Works

Initialization
The game starts with the variable nextPlayer set to 'X'.
The createGameBoard function generates the game board buttons.
Gameplay
Players take turns clicking buttons on the board.
When a button is clicked:
The button's text is updated with the current player's symbol ('X' or 'O').
The button is disabled to prevent multiple clicks.
The turn switches to the next player.
Game End
The isGameOver function checks if all buttons are disabled.
If true, the label with ID game-over-lbl displays "Game Over".
Implementation Details

Functions
createGameBoard()
Dynamically creates the game board buttons and adds them to the DOM.
takeCell(event)
Handles button clicks:
Updates the button's text with the current player's symbol.
Disables the button.
Checks if the game is over.
isGameOver()
Returns true if all buttons are disabled, false otherwise.
Instructions

Setup
Include this script in an HTML file with a game board container and a label with ID game-over-lbl.
Start the Game
Load the HTML file in a browser.
The game board will be created dynamically.
Play
Click on the buttons to take turns as 'X' and 'O'.
Game Over
When all buttons are clicked, the game ends, and "Game Over" is displayed.
