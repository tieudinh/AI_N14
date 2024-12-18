# AI_N14

`cd` to `search` or `multiagent` to run the code inside

## search
```
a. breadthFirstSearch, depthFirstSearch, uniformCostSearch
b. A*Search, CornersProblem
c. cornersHeuristic
d. FoodSearchProblem
e. findPathToClosestDot
```

### Auto grader
```
python python autograder.py
```

### a. breadthFirstSearch, depthFirstSearch, uniformCostSearch.
#### Question 1: Finding a Fixed Food Dot using Depth First Search
```
python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent
```

#### Question 2: Breadth First Search
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5
python eightpuzzle.py
```

#### Question 3: Varying the Cost Function
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
python pacman.py -l mediumDottedMaze -p StayEastSearchAgent
python pacman.py -l mediumScaryMaze -p StayWestSearchAgent
```

### b. A*Search, CornersProblem

#### Question 4: A* search
```
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
```

#### Question 5: Finding All the Corners
```
python pacman.py -l tinyCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
python pacman.py -l mediumCorners -p SearchAgent -a fn=bfs,prob=CornersProblem
```

### c. cornersHeuristic

#### Question 6: Corners Problem: Heuristic
```
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
```

### d. FoodSearchProblem

#### Question 7: Eating All The Dots
```
python pacman.py -l testSearch -p AStarFoodSearchAgent
python pacman.py -l trickySearch -p AStarFoodSearchAgent
```

### e. findPathToClosestDot

#### Question 8: Suboptimal Search
```
python pacman.py -l bigSearch -p ClosestDotSearchAgent -z .5
```

## multiagent
```
f. ReflexAgent
```

### Auto grader
```
python autograder.py -q q1 --no-graphics
```

### f. ReflexAgent

#### Question 1: Reflex Agent
```
python pacman.py -p ReflexAgent -l testClassic
python pacman.py --frameTime 0 -p ReflexAgent -k 1
python pacman.py --frameTime 0 -p ReflexAgent -k 2
```
