# Pacman Search Project

## Overview

This project implements various search algorithms to help Pacman navigate through mazes efficiently. The implementation includes depth-first search, breadth-first search, uniform cost search, and A* search algorithms, along with custom heuristics for solving complex path-finding problems.

## Project Structure

### Core Files to Modify

- `search.py`: Contains search algorithm implementations
  - Depth-First Search (DFS)
  - Breadth-First Search (BFS)
  - Uniform Cost Search (UCS)
  - A* Search
- `searchAgents.py`: Contains search agents and heuristics
  - CornersProblem implementation
  - Corners heuristic
  - Food search heuristic
  - ClosestDotSearchAgent

### Supporting Files

- `pacman.py`: Main game engine
- `game.py`: Game logic and supporting types
- `util.py`: Data structures for search algorithms
- Various display and agent files

## Installation

1. Download the project files
1. Ensure Python 2.7 is installed
1. Extract the files to your preferred directory

## Running the Game

### Basic Commands:

```
# Play basic gamepython pacman.py# Run with specific layout and agentpython pacman.py --layout testMaze --pacman GoWestAgent# View all optionspython pacman.py -h
```

### Testing Search Algorithms:

```
# Test DFSpython pacman.py -l tinyMaze -p SearchAgent# Test BFSpython pacman.py -l mediumMaze -p SearchAgent -a fn=bfs# Test UCSpython pacman.py -l mediumDottedMaze -p StayEastSearchAgent# Test A* Searchpython pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
```

## Project Questions and Features

1. **DFS Implementation (Q1)**

- Implements graph-search DFS
- Avoids expanding visited states
- Returns valid action sequence to goal

1. **BFS Implementation (Q2)**

- Implements graph-search BFS
- Finds shortest path in terms of actions
- Works with Eight Puzzle problem

1. **Uniform Cost Search (Q3)**

- Implements UCS with custom cost functions
- Handles different maze scenarios
- Supports various search agents

1. _A Search (Q4)_*

- Implements A* with heuristic functions
- Uses Manhattan distance heuristic
- Optimizes search efficiency

1. **Corners Problem (Q5-Q6)**

- Custom state representation
- Efficient corner-finding implementation
- Non-trivial admissible heuristic

1. **Food Search (Q7)**

- Optimal food dot collection
- Custom food search heuristic
- Handles complex maze scenarios

1. **Suboptimal Search (Q8)**

- Implements closest dot search
- Provides quick, reasonable solutions
- Handles large maze scenarios


