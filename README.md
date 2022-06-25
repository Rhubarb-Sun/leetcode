# leetcode
Intro: archive the problems

## Maximum Subarray: array, dynamic processing
Explanation: When it comes to the processing of subarray in a array, we can use the idea of dp to **divide the problem to subproblems which focus on the result ending at index i**

transfer equation: `dp[i] = func(dp[i - 1] & arr[i], arr[i])`

[E][53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)

[H][2272. Substring With Largest Variance](https://leetcode.com/problems/substring-with-largest-variance/)

[Medium][474. Ones and Zeroes](https://leetcode.com/problems/ones-and-zeroes/)
(When two factors influence each other, we could think of a 2D array for DP, so that each factor corresponds to every possible situations of the other factor.)

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


## largest ascending path: bfs, dp, memo
Explanation: 
It's easy to figure out that there are some repeated enqueuing in BFS method, so we can use memo to record all the searched nodes. 
Or we can use DP and reorder the node by descending order.

[Hard][329. Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix/)


## carpet covers tiles: sliding window, greedy algorithm, preSum
Explanation: first we order the array by left boundary, then we find out the local optimization is when the left edge of a carpet is aligned with each left side of the tile, this is the idea of a greedy algorithm. So we can use a sliding window and pre-sum to speed up the processing of matching the global maximum.

[M+][2271. Maximum White Tiles Covered by a Carpet](https://leetcode.com/problems/maximum-white-tiles-covered-by-a-carpet/)


## minimums of subarrays: monotonic stack
[M+][907. Sum of Subarray Minimums](https://leetcode.com/problems/sum-of-subarray-minimums/)


## Longest increasing subsequence: dp, binary search
Explanation: we build a dp where dp[i] records the smallest end number of subsequnces of length i + 1, and use binary search to reduce the time complexity. for each number in an array, we always want to find that *dp[i-1] < num <= dp[i]*, so we can update the dp[i] with *num*, or increase the len of dp when num > dp[len].

[M][300. Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/)

[H-][354. Russian Doll Envelopes](https://leetcode.com/problems/russian-doll-envelopes/)


## 扫描线/差分数组
Explanation: when we only care the merge of the intervals.

[E][1893. Check if All the Integers in a Range Are Covered](https://leetcode.com/problems/check-if-all-the-integers-in-a-range-are-covered/submissions/)

## BFS

[H-][2290. Minimum Obstacle Removal to Reach Corner](https://leetcode.com/problems/minimum-obstacle-removal-to-reach-corner/)

## Greedy Algorithm

[M][665. Non-decreasing Array](https://leetcode.com/problems/non-decreasing-array/)

[H][630. Course Schedule III](https://leetcode.com/problems/course-schedule-iii/)


