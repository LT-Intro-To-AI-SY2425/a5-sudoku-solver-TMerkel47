# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

Depth-First Search is overall more efficient and quicker at solving the sodoku problem due to it's heuristic approach as compared to Breadth-First search which would take longer due to it exploring all possible outcomes rather than just following the first one that works. In situations where you need to search for a solution quickly DFS is the way to go. In situations where the problems requires you to find all solutions or the most efficient path possible BFS is superior.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Due to the say that DFS works, the stack is crucial to it working as it allows the DFS to explore all nodes for a branch before moving on the to next in the LIFO way. The same can be said for BFS and the queue structure as it allows for the BFS to search all nodes for a depth before moving on to the next depth in the FIFO way. The only alternatives I could think of would be if you were to have a priority queue or stack that would make the code more efficient.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

Well the most simple way it can be adapted is just by making it larger so it could handle larger puzzles or grids. You could also change the data types used so the code could be used for different uses other than solving a sodoku puzzle such as following a pattern. This could be applied in a number of ways from routing connections on the internet to be as efficient as possible to finding the easiest path to take on an app like google maps.