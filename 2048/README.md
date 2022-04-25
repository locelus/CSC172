To run this game, simply run the main function inside the Game class. The game starts by generating a 4x4 grid with 2 random positions filled with either a 2 or a 4. There is a 20% chance of the number being a 4 and an 80% chance of the number being a 2. The game then prints the grid to console. Then, input is gotten from the user. If the input is a w, a, s, or d, all items on the board are moved in the respective direction. For example, if the user presses w, the following happens. The game loops from bottom to top of all columns on the grid, moving a number up if a number is encountered and it is possible to move up. The conditions for a number to move up are: There must either be a 0 or the same number above the current number. If it is the same number (for example a 4 above a 4) the 4 is moved upwards into the other 4 and turns into an 8. If the number above is a 0 (blank), the 4 is moved up into the 0, changing the 0 to a 4. Either way, the spot vacated by the 4 is made blank after it moves. If a move was not made at any point during the process, this direction was not a valid move. If a valid move was not made, the game will inform the user that the move was not valid and prompt the user for another direction. If a valid move was made, the game continues with the turn, iterating the moves made variable to keep track of the total moves made. It then "clears" the console by outputting multiple blank lines, and then prints the debug statements of the maximum number on the board and the total number of moves made so far. Then, if the user has not won or lost, the game continues in this loop, reprinting the board and getting input from the user until the user has won or lost. If the user has won (i.e. 2048 is somewhere on the board) the game congratulates the user and asks if they would like to play again, and takes the according action depending on player input. If the user has lost (i.e. there are no more valid moves on the board to be made) the game informs the user and asks if they would like to play again, and takes the according action depending on player input. When the player is prompted for a move, they can also input q or r instead of a move direction. q will ask the user to confirm quitting the game, and quit if the user confirms. r will ask the user to confirm restarting the game, and will restart if the user confirms. If the user does not input w, a, s, d, r, or q when prompted for a move, the game will inform the  user they have made an invalid move and prompt them for another input until they enter a valid input.