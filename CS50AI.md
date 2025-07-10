## Search Problems
Graph Search Algorithms (e.g., BFS, DFS) 
Useful in robotics, pathfinding (games), recommender systems etc.
Example: maze path, google map paths, solve a word puzzle tile

Initial State: Initial state, or the current state of a puzzle
Action: a move in the puzzle, which results in another state. 
Transition Model: The result_function(stateX, action/move) => stateY
Goal Test: How does AI determine this state is the final outcome
Path Cost Function: Numerical cost associated with the given path to identify the best possible path

### Solution algorithm 
- Start with a frotier (the node or set of nodes that are being worked on in the graph) that cotains the initial state
- Start with an empty explored set (a set to keep track of what nodes have been explored already)
- Repeate:
  - if the frontier is empty, then no solution
  - remove a node from the frontier
  - if node contains goal state (i.e. target), return the solution
  - add the node to the explored set
  - expand node, add resulting nodes to the frontier if they aren't already in the frontier or the explored set

#### Possible algorithms
- Depth-first search: it goes all the way to the leaves to check the target or dead end. This may not always find the best path.
- Breath-first search: it checks the next node in all branches. it needs to explore lost of states
