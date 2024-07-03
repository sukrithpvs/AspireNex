# AspireNex

# Tic-Tac-Toe AI Game

## Overview

This is a simple Tic-Tac-Toe game created using Python and Tkinter. You can play against a computer AI that uses the Minimax algorithm to make its moves.

## How to Run

1. **Ensure you have Python installed.**
2. **Run the game:**
    ```bash
    python tictactoe.py
    ```

## How to Play

1. **Choose Your Side:**
   - Select 'X' or 'O' and click "Start Game".

2. **Choose Who Goes First:**
   - Decide if you want to start first or let the computer go first.

3. **Make Your Move:**
   - Click on an empty cell to place your mark.
   - The computer will make its move automatically.

4. **Reset the Game:**
   - Click "Reset" to start a new game.

## Code Explanation

### Key Functions

- **evaluate(state):** Evaluates the board state.
- **wins(state, player):** Checks if a player has won.
- **game_over(state):** Checks if the game is over.
- **empty_cells(state):** Returns a list of empty cells.
- **valid_move(x, y):** Checks if a move is valid.
- **set_move(x, y, player):** Sets a move on the board.
- **minimax(state, depth, player):** Minimax algorithm for AI moves.
- **ai_turn():** Handles AI's turn.
- **human_turn(x, y):** Handles human's turn.
- **render():** Updates the GUI.
- **check_game_over():** Checks and displays game result.
- **on_click(row, col):** Handles cell clicks.
- **reset_game():** Resets the game state.
- **start_game():** Starts the game with chosen settings.
- **show_choice_frame():** Displays initial choices.

### GUI Setup

- **Main Window:** Created using Tkinter.
- **Choice Frame:** Lets you choose 'X' or 'O' and who goes first.
- **Game Frame:** Displays the Tic-Tac-Toe board and controls.

## License

This project is open-source and can be freely modified or distributed.

Enjoy playing Tic-Tac-Toe!
