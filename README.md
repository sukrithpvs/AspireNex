# AspireNex
# Image Captioning with PyTorch

This project demonstrates how to train an image captioning model using PyTorch. The model combines a pre-trained ResNet for image encoding and a pre-trained GPT-2 language model for caption generation.

## Requirements

- Python 3.x
- PyTorch
- Torchvision
- Transformers
- Pandas
- Pillow
- Gradio (optional)


## Usage

1. **Prepare the dataset**:
   - Set the paths for the `images_folder` and `captions_file` variables in the code.
   - Ensure the dataset is structured as mentioned above.

2. **Train the model**:
   - Run the code to start the training process.
   - The model will be trained for 25 epochs, and the training and validation losses will be displayed after each epoch.
   - The trained model will be saved as `image_captioning_model.pth`.

3. **Generate captions**:
   - The code includes a `generate_caption_for_image` function that takes an image path and generates a caption using the trained model.
   - You can call this function with an image path to generate a caption for a specific image.

4. **(Optional) Create a Gradio interface**:
   - If you have Gradio installed, you can create an interactive interface to generate captions for uploaded images.
   - Uncomment the `main` function and run the code to launch the Gradio interface.
   - Upload an image, and the generated caption will be displayed.

## Model Architecture

The image captioning model consists of two main components:

1. **ResNet**: A pre-trained ResNet model is used for image encoding. The last fully connected layer and average pooling layer are removed, and the output features are projected to match the size of the GPT-2 hidden state.

2. **GPT-2**: A pre-trained GPT-2 language model is used for caption generation. The image features are added to the input embeddings of the GPT-2 model to incorporate visual information during caption generation.

The combined model is trained end-to-end using the PyTorch framework.

## Acknowledgments

This project is inspired by the image captioning tutorial from the PyTorch documentation and the Hugging Face Transformers library.

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

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/7324171/b0c88bda-b4eb-4d06-bbe1-2bdfedc98d46/paste.txt
