# leetcode
Intro: archive the problems

## Maximum Subarray: array, dynamic processing
Explanation: When it comes to the processing of subarray in a array, we can use the idea of dp to **divide the problem to subproblems which focus on the result ending at index i**

transfer equation: `dp[i] = func(dp[i - 1] & arr[i], arr[i])`

[Easy][53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)

[Hard][2272. Substring With Largest Variance](https://leetcode.com/problems/substring-with-largest-variance/)


## Deepest of a tree: tree, layer order, queue
Explanation: use **layer order with a queue** to reach the deepest layer of a tree.

[Medium][1302. Deepest Leaves Sum](https://leetcode.com/problems/deepest-leaves-sum/)


## transmission time in a graph: Dijkstra's Algorithm
Explanation: build a graph keeps the distance of every two nodes. Each step, find the want-most unvisited node and update the graph.

[Medium][743. Network Delay Time](https://leetcode.com/problems/network-delay-time/)


## shortest path with 8 directions: A* Algorithm
Explanation: An A* search is like a breadth-first seach, except that in each iteration, instead of expanding the cell with the shortest path from the origin, we expand the cell with the **lowest overall estimated path length** -- this is the distance so far, plus a heuristic (rule-of-thumb) estimate of the remaining distance. As long as the heuristic is consistent, an A* graph-search will find the shortest path. This can be somewhat more efficient than breadth-first-search as we typically **don't have to visit nearly as many cells**. Intuitively, an A* search has an approximate sense of direction, and uses this sense to guide it towards the target.

[Medium][1091. Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix/)


## find in a tree: dfs, recursion, preorder
Explanation: if you would like to find something in a tree, a good common solution is to search it recursively while paying attention to the situation that you may encounter the *null* which should be considered as the end of a round of search.

[Medium][1379. Find a Corresponding Node of a Binary Tree in a Clone of That Tree](https://leetcode.com/problems/find-a-corresponding-node-of-a-binary-tree-in-a-clone-of-that-tree/)


## undirected graph: dfs
Explanation: memorize all the neighbors of each node, transverse the graph step by step without going back. The depth of a node is the lowest depth it can travel to. The nodes share the depth shall be in a circle.

[Hard][1192. Critical Connections in a Network](https://leetcode.com/problems/critical-connections-in-a-network/)
