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
