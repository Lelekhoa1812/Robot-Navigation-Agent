# Robot-Navigation-Agent
Python algorithms for robot mapping navigation.

Intelligent robot agent find its way to the goal target by integrating search methods (DFS, BFS, GBFS, A* and custom methods) alongside with heuristic calculation (Manhattan and Euclidean distance).

Map txt file configuration have these components:
[a,b]            // the grid has a rows and b columns
(c,d)            // initial position at cth column and dth row
(e,f) | (g,h)    // goal states 
(i,j,k,l)        // the wall has the leftmost top corner occupies cell (i,j) and is k cell(s) wide and l cell(s) high
/.../            // the rest of entries are for wall configs

GUI display in gui.py using tkinter extension for visualization. It should show all cells the agent has explored (traversed) as purple, all cells to the goal node (path) as yellow, wall(s) as gray and empty cells as white.

Instruction - Run the code using the following format:
python searchmain.py [map file] [search method]
For instance:
python searchmain.py complexmap.txt BFS

A product of COS30019 unit, Swinburne semester 1, 2024.
