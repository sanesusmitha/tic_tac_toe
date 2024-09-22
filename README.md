# tic_tac_toe
This Python code is a simple implementation of the game Tic Tac Toe using the tkinter library for the graphical user interface (GUI) and numpy for numerical operations. The game is played on a 3x3 grid, and two players take turns to place their symbols (X and O) in empty squares. The game ends when either player has three of their symbols in a row, column, or diagonal, or when all squares are filled without a winner.

The code defines a class Tic_Tac_Toe that contains various methods to handle the game logic, drawing symbols on the canvas, checking for winners, and handling user input. Here's a breakdown of what each method does:

__init__(self): Initializes the game window, canvas, and game state variables. It creates a 3x3 grid on the canvas and binds a click event to the canvas.

mainloop(self): Starts the main loop of the game, which runs until the window is closed.

initialize_board(self): Draws the grid lines on the canvas.

play_again(self): Resets the game board and switches the starting player.

draw_O(self, logical_position): Draws an O symbol on the canvas at the specified logical position.

draw_X(self, logical_position): Draws an X symbol on the canvas at the specified logical position.

display_gameover(self): Displays the game over message and updates the scores.

convert_logical_to_grid_position(self, logical_position): Converts a logical position (row and column) to a grid position (pixel coordinates).

convert_grid_to_logical_position(self, grid_position): Converts a grid position (pixel coordinates) to a logical position (row and column).

is_grid_occupied(self, logical_position): Checks if a grid square is occupied by a symbol.

is_winner(self, player): Checks if a player has won the game.

is_tie(self): Checks if the game is a tie.

is_gameover(self): Checks if the game is over (either a winner or a tie).

click(self, event): Handles the user's click event. It determines the logical position of the clicked square and draws the appropriate symbol based on the current player. It also checks if the game is over and displays the game over message.

Finally, the code creates an instance of the Tic_Tac_Toe class and starts the main loop using the mainloop() method.
