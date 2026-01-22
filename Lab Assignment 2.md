

|**Variables**|**What it represents**|**Data Structure**|
|-|-|-|
|game\_grid|The 3x3 playing grid|two-dimensional array or matrix|
|dimensions|The dimensions of the playing grid|number|
|player1\_mark|The symbol used by player1 ('X')|string or number|
|player2\_mark|The symbol used by player2 ('O')|string or number|
|current\_player\_turn|The current turn of the player|number|
|player1\_move|The position of player1's current move|array with 2 values (row and column of grid)|
|player2\_move|The position of player2's current move|array with 2 values (row and column of grid)|
|outcome|The current outcome of the game (player1 winner, player2 winner. tie, unfinished)|string or number|
|**Loops**|**What it represents**|**Data Structure**|
|Player Turn Loop|The players switching turns after the they take their turn.|If-Else Statement, using the current\_player\_turn variable.|
|End Game Check|The players seeing if a game-ending match has been made.|If-Else statement, using the game\_grid variable. Produces outcome.|
|Position Filled Check|If the spot the player wishes to use is already in use.|For Statement, using the playerX\_move arrays|





Start Game
2. Declare Variables
3. Loop until End Game Check gets an outcome that is not unfinished
4. Current Player turn
5. &nbsp;	Current Player Move
6. &nbsp;		Players presses up arrow, move mark position up
7. &nbsp;		Players presses down arrow, move mark position down
8. &nbsp;		Players presses left arrow, move mark position left
9. &nbsp;		Players presses right arrow, move mark position right
10. &nbsp;		Players presses space, confirm mark position 
11. &nbsp;			Do Position Filled Check
12. &nbsp;	Position Filled Check
13. &nbsp;		If column \& row not filled, mark position
14. &nbsp;		If they are, tell player to choose new spot
15. &nbsp;			Return to Current Player Move
16. &nbsp;	Do End Game Check
17. &nbsp;		If all marks in a column, row, or diagonal are the same, current player wins
18. &nbsp;		No more spaces available, tie
19. &nbsp;	Change current player variable
