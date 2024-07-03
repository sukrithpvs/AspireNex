# AspireNex: Image Captioning with PyTorch

This project demonstrates how to train an image captioning model using PyTorch, combining a pre-trained ResNet for image encoding and a GPT-2 model for caption generation.

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
   - Set paths for `images_folder` and `captions_file`.
   - Ensure the dataset structure is correct.

2. **Train the model**:
   - Run the training code for 25 epochs.
   - Model saved as `image_captioning_model.pth`.

3. **Generate captions**:
   - Use `generate_caption_for_image` function with an image path.

4. **(Optional) Create a Gradio interface**:
   - Uncomment the `main` function to launch Gradio interface.
   - Upload an image to get captions.

## Model Architecture

1. **ResNet**: Pre-trained ResNet for image encoding. Output features match GPT-2 hidden state size.
2. **GPT-2**: Pre-trained GPT-2 for caption generation. Image features are added to GPT-2 input embeddings.

## Acknowledgments

Inspired by PyTorch tutorials and Hugging Face Transformers library.

---

# Face Recognition System using ArcFace

This project uses ArcFace for face recognition with additional features like facial expression recognition and gender detection.

## Requirements

- Python 3.6 or higher
- PyTorch
- OpenCV
- NumPy

Install dependencies:

```bash
pip install torch torchvision opencv-python numpy
```

### Setup

1. **Download Pre-trained Model**: Place `backbone_r100.pth` in the directory. [Download here](https://github.com/deepinsight/insightface).

2. **Clone Repository**:

```bash
git clone https://github.com/your-username/arcface-face-recognition.git
cd arcface-face-recognition
```

3. **Place Haarcascade XML File**: Download `haarcascade_frontalface_default.xml` from [OpenCV GitHub](https://github.com/opencv/opencv/tree/master/data/haarcascades).

## Usage

1. Connect your webcam.
2. Run `face_recognition.py`.
3. Press 'q' to quit the video feed.

## License

MIT License.

## Acknowledgments

- [InsightFace](https://github.com/deepinsight/insightface)
- [OpenCV](https://opencv.org/)

---

# Tic-Tac-Toe AI Game

This is a simple Tic-Tac-Toe game using Python and Tkinter with a Minimax algorithm AI.

## How to Run

1. **Ensure Python is installed.**
2. **Run the game**:

```bash
python tictactoe.py
```

## How to Play

1. **Choose Your Side**: Select 'X' or 'O' and click "Start Game".
2. **Choose Who Goes First**.
3. **Make Your Move**: Click an empty cell to place your mark.
4. **Reset the Game**: Click "Reset" to start a new game.

## Code Explanation

### Key Functions

- `evaluate(state)`: Evaluates the board state.
- `wins(state, player)`: Checks if a player has won.
- `game_over(state)`: Checks if the game is over.
- `empty_cells(state)`: Returns empty cells.
- `valid_move(x, y)`: Checks move validity.
- `set_move(x, y, player)`: Sets a move.
- `minimax(state, depth, player)`: Minimax algorithm for AI.
- `ai_turn()`: Handles AI's turn.
- `human_turn(x, y)`: Handles human's turn.
- `render()`: Updates the GUI.
- `check_game_over()`: Displays game result.
- `on_click(row, col)`: Handles cell clicks.
- `reset_game()`: Resets the game state.
- `start_game()`: Starts the game with chosen settings.
- `show_choice_frame()`: Displays initial choices.

### GUI Setup

- **Main Window**: Created using Tkinter.
- **Choice Frame**: Choose 'X' or 'O' and who goes first.
- **Game Frame**: Displays the Tic-Tac-Toe board and controls.
