# Heuristic Analysis

This work presents 3 heuristics for achieving better performance than the `ID_Improved` agent. Each one increases the complexity in terms of computation and implementation. Let's analyze each one:

## Center moves

### Intuition

The more moves at the center this player has, the better the outcome of the game will be.

### Implementation

This function simply subtracts the opponent's center moves from the player's center moves. Center moves are defined as the inner `3x3` rectangle of the board.

## Center moves with blank spaces

### Intuition

Same as the above but we scale according to the available blank squares.

### Implementation

Call `center_moves()` and divide the result by the number of blank squares.
