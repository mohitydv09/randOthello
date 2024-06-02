# RandOthello Game Module

This is my implementation of the famous game RandOthello. I have implemented various players to play the game, including:
-RandomPlayer: A player that makes random moves from legal actions.
-HumanPlayer: A player that allows human input for moves.
-MinimaxPlayer: A player implementing the Minimax algorithm for decision-making.
-AlphaBetaPlayer: A player implementing the Alpha-Beta Pruning algorithm for optimized decision-making.

I followed the template from the book "Artificial Intelligence: A Modern Approach, Global Edition" by Peter Norvig and Stuart Russell.

## Modifications from normal RandOthello

This implementation has added complexity where at the game's start, we choose a random square in the top row and a random square in the bottom row and block those out as unplayable locations. This forces us to come up with new heuristics that are not commonly available online.

## Usage
By default, the code is set to play between a human player and an AI agent using the Minimax algorithm with Alpha-Beta pruning, allowing a lookahead depth of 5 and still running in under 1 second. This can be changed in the main() function.

Default Configuration:
Where WHITE and BLACK are players and 5 is the depth up to which the Minimax agent looks ahead
```
play_game(p1=MinimaxPlayer(BLACK,5),p2=HumanPlayer(WHITE))
```
