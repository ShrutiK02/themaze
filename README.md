# themaze
Maze Solver using BFS and DFS

This project provides Python implementations for solving the LeetCode problem [490. Maze](https://leetcode.com/problems/the-maze/). It includes two solutions: one using Breadth-First Search (BFS) and another using Depth-First Search (DFS).

## Problem Description
Given a maze represented by a 2D array where 0s represent empty spaces and 1s represent walls, along with a starting position and a destination, determine if there is a path from the starting position to the destination. 

## Usage
The provided code includes two classes `BFS_Solution` and `DFS_Solution`, each with a method `hasPath()` to solve the problem using BFS and DFS respectively. Both methods take the following arguments:
- `maze`: A list of lists representing the maze.
- `start`: A list containing the starting position coordinates.
- `destination`: A list containing the destination position coordinates.

### Example
```python
from maze_solver import BFS_Solution, DFS_Solution

maze = [
    [0, 0, 1, 0, 0],
    [0, 0, 0, 0, 0],
    [0, 0, 0, 1, 0],
    [1, 1, 0, 1, 1],
    [0, 0, 0, 0, 0]
]
start = [0, 4]
destination = [4, 4]

bfs_solver = BFS_Solution()
dfs_solver = DFS_Solution()

print("BFS Solution:", bfs_solver.hasPath(maze, start, destination))  # Output: True
print("DFS Solution:", dfs_solver.hasPath(maze, start, destination))  # Output: True
