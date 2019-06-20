# Chess

## Steps

### Movement constraints

Implement the following function:
```elm
possibleMovements : Board -> Piece -> List Cell
```
This function compute possible movements for a given piece. It must switch over every piece. For every piece, we should use subfunctions like the following:
```elm
possibleKingMovements : Board -> List Cell
```
#### Knight movements
Compute possible coordinates:
```elm
computePossibleKnightMovementCoordinates : (Int, Int) -> List (Int, Int)
```
Exclude not possible coordinates (outside the board, or same color pieces)
```elm
validateCoordinates : Board -> Cell -> List (Int, Int)
```
#### Pawn movements
We have to figure a way to track if a pawn has done a 2 cell forward movement or not. We could use a boolean on every Pawn, or track pawns that just did it. Pawn possible movements depend on the color.
We could implement something like:
```elm
computePossiblePawnMovements : (Int, Int) -> Color -> Bool -> List (Int, Int)
```