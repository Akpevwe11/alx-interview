## n queeens problem 

The n-queens problem invoves arranging the queens in such a way that none of the queens is under attack. 

For any of the queen to be under attack, the following conditions must be satisfied: 

[x] No two queen must be  on the same row

[x] No two queen must be on the same column

[x] No two queen must be arranged diagonally

N.B: These all happens in a 4 x 4 Chess board. 

so in a 4 x 4 chess board, what are the ways in which the queens can be placed? 

They can be placed in `16C4` ways 
    1   2    3      4
 ______________________
|     |    |    |      |    1  
|_____|____|____|______|
|     |    |    |      |
|_____|____|____|______|    2
|     |    |    |      |
|_____|____|____|______|    3
|     |    |    |      |
|_____|____|____|______|    4


The solution to this problem, is to use backtracking.


The N-Queens problem is a classic example of using backtracking to find solutions. The problem is to place N queens on an N×N chessboard so that no two queens threaten each other. This means that no two queens can be in the same row, column, or diagonal.

Here is a step-by-step approach to solving the N-Queens problem using the backtracking method in Python:


1. Define the Problem:

   [x] Place N queens on an N×N chessboard.

   [x] Ensure no two queens can attack each other.


2. Backtracking Approach:

  [x]  Place queens column by column.

  [x] Use a recursive function to try placing a queen in each row of the current column.

  [x]  If placing a queen in the current row and column does not lead to a conflict with  already placed queens, move to the next column.

  [x]  If all columns are successfully filled, print the board configuration.

  [x]  If placing the queen leads to a conflict, backtrack by removing the queen and trying the next row.


What is Back Tracking? 

Backtracking means just what it sounds like. In some problems, as we sarch for a solution we may reach a 
dead end and have to go back. back tracking is ususally associated with recursion. 



