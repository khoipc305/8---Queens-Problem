# 8---Queens-Problem
Assignment - 1
1. Write a GUI based program that can place 8 queens in such a manner on an 8 x 8 chessboard that no queens attack each other.

2. Use a heuristic function for the 8-queens problem that estimates how close a given board state is to a solution. The goal state is one where no queens are attacking each other.

 

Example Heuristic Function: Number of attacking pairs of queens

The function counts the total number of pairs of queens that are currently attacking each other.

A pair of queens is considered "attacking" if they are in the same row, same column, or on the same diagonal.

The goal state has a heuristic value of 0, as there are no attacking pairs.

A state with a high number of attacking pairs is considered "bad" and a state with a low number is considered "good."

When using this heuristic with a greedy search algorithm, you would always choose to move a queen in a way that minimizes the number of attacking pairs on the board. A greedy search using this heuristic will continuously move toward the goal.

When using this heuristic with an A* search algorithm, the evaluation function would be:

f(n)=g(n)+h(n)

g(n) is the cost of the path so far, which can be defined as the number of moves made to reach the current state.

h(n) is the heuristic value, which is the number of attacking queen pairs.
