# TIC-TAC-TOE

This repositary contains the code for Tic-Tac-Toe game. The game is player in 3 ways:
1. Human vs Human
2. Human vs Computer
3. Computer vs Computer
## Steps Involved
- Define function **win**: compare the passed array items to check whether all contains the same value and return the winner
- Define a function to **validate** the game
  - check for the row: extract each row and check by calling the win function
  - check for column: run a nested for loop one in range of size and another for row. Append the value from row by index of first loop. feed the column array to function win
  - Check for forward diagonal: As there is only 1 forward diagonal provide the diagonal, extract the values by provide the idex directly and feed the extracted array to the win function
  - Check for Backward diagonal: Similar to forward diagonal, extract values using index value directly and feed the values to the win function
- Define function to **print the Tic Tac Toe board**
- Function to Update the board:  Creating list of all the position in the boards: the list is 2D where the each item contains 2 values representing rows and columns respectively, Update the board with the new values
- Function to implement a **game between Human and Human**:
  - Intialize a board with the position values
  - intitalize a list with player names
  - run a for loop with size of number of boxes i.e 9
  - Get the input position value from user based on the player index
  - Update the board according to the input position
  - Check for validate function if for loop index is more than or equal to 4
  - if got a return value print the winner and then exit the for loop
  - if for loop is finished without printing the winned then Print "Its a tie"
- Function to implement a **game between human and computer**
  - Most of the work are similar to human vs Human except using random function
  - Created a list containing number of choices
  - Run a for loop with size 9
  - Get the input from user and remove that position from the list of choices
  - randomly choose the value from choices list using random function and removed the choosed position from the list
  - Call for validate function
- Function to implement **game of Computer vs Computer game**:
  - ALl the same with the above function except that the both input is taken randomly from the choices list using random function    
