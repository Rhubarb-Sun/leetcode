# leetcode
archive the problems

## Maximum Subarray
** When it comes to the processing of subarray in a array, we can use the idea of dp to divide the problem to subproblem which focuses on the result ending at index i.**
transfer equation: `dp[i] = func(dp[i - 1] & arr[i], arr[i])`

[53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)
[2272. Substring With Largest Variance](https://leetcode.com/problems/substring-with-largest-variance/)
