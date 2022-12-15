# Connect 4
A game of Connect 4 written in Python. Players take turns dropping a piece on the board, and the first one that connects 4 wins.

## Usage
The users can change the game settings before launching the game (e.g., choosing between playing the game in the console or in a GUI, each player's name and whether they are controlled by an AI or not, and the strategy used by the AI for each player). This can be done by modifying the ```settings.properties``` file from the ```Data``` folder. The default settings are the following:

## AI Implementation
The AI analyses every possible move from the current board state by using a minimax algorithm, trying to maximize the score of its moves and minimizing the score of the opponent's moves. In the case of this game, the score depends on the placement of the pieces and the possibilities of placing 4 pieces of one color in a row. The AI only simulates 3 moves in advance, since any more moves would seriously hurt the time performance. This way, it decides which move is the most profitable, and uses it once the computations are done. 