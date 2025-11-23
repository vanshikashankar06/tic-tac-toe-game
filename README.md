# Tic Tac Toe Game

A classic Tic Tac Toe game built with Pygame, featuring a clean graphical interface and smooth gameplay for two players.

## Features

- **Graphical Interface**: Beautiful teal-themed board with smooth graphics
- **Two-Player Gameplay**: Play with a friend on the same computer
- **Visual Feedback**: Clear X and O symbols with distinct colors
- **Win Detection**: Automatically detects wins and tie games
- **Game Reset**: Quick restart with a single key press
- **User-Friendly**: Simple click-to-play interface

## Requirements

- Python 3.x
- Pygame library

## Installation

1. **Install Python** (if not already installed):
   - Download from [python.org](https://www.python.org/downloads/)
   - Make sure to check "Add Python to PATH" during installation

2. **Install Pygame**:
   ```bash
   pip install pygame
   ```

## How to Run

1. Save the code to a file (e.g., `tictactoe.py`)
2. Open your terminal/command prompt
3. Navigate to the directory containing the file
4. Run the program:
   ```bash
   python tictactoe.py
   ```

## How to Play

### Basic Rules
- The game is played on a 3x3 grid
- Player X goes first, followed by Player O
- Players take turns clicking on empty squares
- First player to get 3 in a row (horizontally, vertically, or diagonally) wins
- If all squares are filled with no winner, the game is a tie

### Controls
- **Mouse Click**: Click on any empty square to place your mark (X or O)
- **R Key**: Press 'R' to restart the game after it ends
- **Close Window**: Click the X button to exit the game

### Game Flow
1. Game opens with an empty 3x3 grid
2. Player X clicks a square to make the first move
3. Player O clicks a square to make their move
4. Continue taking turns until someone wins or the board is full
5. When the game ends, a message displays the winner or announces a tie
6. Press 'R' to play again

## Game Elements

### Visual Design
- **Background**: Teal color for a modern look
- **Grid Lines**: Darker teal lines dividing the board
- **X Symbol**: Dark gray crossing lines
- **O Symbol**: Light beige circle
- **Game Over Screen**: Semi-transparent overlay with winner announcement

### Win Conditions
The game checks for wins in:
- All 3 horizontal rows
- All 3 vertical columns
- 2 diagonal lines (top-left to bottom-right, top-right to bottom-left)

## Code Structure

### Main Components
- **Board**: 3x3 list storing game state ('X', 'O', or empty)
- **draw_grid()**: Draws the game board lines
- **draw_symbols()**: Renders X and O marks on the board
- **check_winner()**: Checks all win conditions
- **check_tie()**: Determines if the game is a tie
- **show_game_over()**: Displays end game message
- **reset_game()**: Clears the board for a new game

### Game Loop
The main loop continuously:
1. Checks for user input (clicks and key presses)
2. Updates the game state
3. Redraws the display
4. Checks for win/tie conditions

## Customization

You can easily customize the game by changing these values:

### Colors (RGB format)
```python
background_color = (28, 170, 156)   # Board background
line_color = (23, 145, 135)         # Grid lines
x_color = (66, 66, 66)              # X symbol color
o_color = (239, 231, 200)           # O symbol color
```

### Window Size
```python
width = 600   # Window width in pixels
height = 600  # Window height in pixels
```

### Line Thickness
Change the last parameter in `pygame.draw.line()` and `pygame.draw.circle()` calls

## Troubleshooting

### "pygame not found" error
- Make sure Pygame is installed: `pip install pygame`
- Try: `pip3 install pygame` if using Python 3

### Game window doesn't open
- Check that you have Python 3.x installed
- Ensure no firewall is blocking the application

### Clicks not registering
- Make sure you're clicking inside the game window
- Click in the center of squares for best results

## Future Enhancements

Possible improvements for future versions:
- Single-player mode with AI opponent
- Difficulty levels (Easy, Medium, Hard)
- Score tracking across multiple games
- Animation effects for moves and wins
- Sound effects for moves and wins
- Custom player names
- Different board sizes (4x4, 5x5)
- Online multiplayer capability
- Theme customization menu

## Learning Objectives

This project demonstrates:
- Pygame basics (window creation, event handling, drawing)
- 2D list/array manipulation
- Game loop implementation
- User input handling
- Collision detection (click to grid conversion)
- Game state management
- Win condition algorithms

## License

Free to use and modify for educational purposes.

## Credits

Built with Python and Pygame for learning and entertainment.
