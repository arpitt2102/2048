# 2048 Game
### How to play:

In order to perform a left swipe, we will first compress and then merge the gridCell matrix. If either of these operations returns true (meaning the values of the matrix were impacted by the previous two functions), we then need to compress the grid once more.
We'll take transpose to move up, swipe left to go back to the previous order, and then take transpose once more.
Moving up and down are equivalent, but the matrix needs to be turned around.
Moving right is equivalent to moving left plus reverse.
After each operation, we must check the game's status. If all the cells are occupied and we are unable to even merge any two cells, the game is over because no movement can alter the matrix.

If any cell value has reached 2048, then the player is won and a message box is flashed on the screen announcing the winner.

### Running it on your local machine:
```
python3 2048.py
```
