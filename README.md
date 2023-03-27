# Battleship-Game

Battleship is a classic two-player guessing game where each player attempts to sink the other's hidden fleet of ships. The game is typically played on a grid board, and each player has their own board where they place their ships. Players take turns guessing the location of their opponent's ships by calling out the coordinates of a square on the grid. The opponent responds with "hit" or "miss," and the player marks their own board accordingly. The first player to sink all of their opponent's ships wins. Battleship can be played on paper, a board game, or online.

## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type python ```battleship.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* Import the ```randint function``` from the ```random module```.

* Create an empty list called ```board```.

* Append six lists of six "O" characters to the board list, creating a ```6x6 grid of "O"s```.

* Define a function called ```print_board``` that takes a board parameter and prints the current state of the board to the console. This function iterates through each row in the board list and prints a space-separated string of the characters in the row.

* Print a message to the console that says ```"Let's play Battleship!"```.

* Call the ```print_board``` function with the board parameter to print the initial state of the board.

* Define a function called ```random_row``` that takes a board parameter and returns a random row index from the board list.

* Define a function called ```random_col``` that takes a board parameter and returns a random column index from the first row of the board list.

* Call the ```random_row``` and ```random_col``` functions to generate random row and column indices for the battleship.

* Use a for loop to iterate through ```9 turns``` of the game.

* Print the current turn number to the console.

* Prompt the user to input a guess for the row and column indices of the battleship.

* If the user's guess matches the row and column indices of the battleship, print a message to the console saying ```"Congratulations! You sunk my battleship!"``` and exit the loop with the break statement.

* If the user's guess does not match the battleship, check if the guess is out of bounds or has already been guessed. If so, print an appropriate message to the console.

* If the guess is valid but misses the battleship, mark the corresponding position on the board with an ```"X"```.

* If the current turn is the last one (turn 8), print ```"Game Over"``` to the console.

* Increment the turn counter.

* Call the ```print_board``` function with the updated board parameter to print the current state of the board.
