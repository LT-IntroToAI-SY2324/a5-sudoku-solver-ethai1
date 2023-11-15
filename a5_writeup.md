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
The performance of DFS and BFS are pretty similiar, at least on these two puzzles, but on the second puzzle, BFS went through nearly a 150 more iterations to find the solution. I even tried using the time module to see how long it took for it to run and they're roughly similiar, with the test cases being milliseconds apart. I think for DFS to be as efficient as possible, it would require a puzzle where it can find the correct possibility almost immediately without having to go through too many different options while BFS woild work better when they're are less possibilities overall for the program to go through and waste time and resources on.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
Using different data strucutures changed how the program went through processing the different boards that had accumulated in the data strcuture and most of the changes were the variable names for the data structure and obviously changing Stack to a Queue in BFS.


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
For larger Sudoku puzzles, we can change the size variable in the board class while for different board games, the board stays mostly the same with perhaps size differences while the code for it is obviously completely different. We can also use DFS and BFS for other algorithms that are perhaps more practical and useful than in a sudoku solver along with data structures that can optimize any program that you want.

