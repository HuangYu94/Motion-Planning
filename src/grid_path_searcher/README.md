# grid_path_searcher
### Build and Run
Build this source code before running according to ROS melodic catkin_make tutorial..
Then run demo node

```
$source devel/setup.bash
$roslaunch grid_path_searcher demo.launch
```
What you will get after click on a valid goal grid
![](./AStar_show_all_visited.png "A* algorithm showing all visited node")
A\* algorithm showing all visited node

![](./JPS_show_all_visited.png "JPS algorithm showing all visited node")
JPS algorithm showing all visited node

![](./only_show_path.png "A* algorithm showing planned path only")
A\* algorithm showing planned path only

### Interesting Facts

Following pictures demonstrated that when obstacles step in the path from start point to goal point, A\* with Manhattan heuristics will find suboptimal path after searching a small space; while A\* with Euclidean heuristics will tend to find the optimal path after searching a larger space.

![](./euclidean_path.png)
A\* using Euclidean Heuristic finds the optimal path
![](./euclidean_visited.png)
A\* using Euclidean Heuristic finds the optimal path searched 5317 grids


![](./manhattan_path.png)
A\* using Manhattan Heuristic finds the suboptimal path
![](./manhattan_visited.png)
A\* using Manhattan Heuristic finds the suboptimal path searched 2384 grids