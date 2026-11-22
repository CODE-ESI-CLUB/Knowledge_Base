# Session Planning

> **Goal:** prepare club members for technical interviews first, then competitive programming contests.
> **Language:** Python (C++ is taught in parallel).
> **Rhythm:** one session per week

## Session 0: Kick-off
**Objectives:** understand what CP and coding interviews are, set up tools, learn how to practise.
- What is competitive programming? CP vs. technical interviews
- Club objectives
- Platforms: LeetCode (interviews), Codeforces (contests)
- Python essentials for problem solving: lists, slicing, comprehensions, `dict`, `set`, `sorted`, `enumerate`, `zip`

**Problems:** Two Sum (LC 1) · Contains Duplicate (LC 217) · Fizz Buzz (LC 412)

## Session 1: Complexity, Arrays & Hashing
**Objectives:** estimate complexity from constraints, use hash maps to go from O(n²) to O(n).
- Big-O time & space, best/worst case
- Constraints → target complexity (n ≤ 10⁵ → O(n log n), n ≤ 20 → O(2ⁿ) …)
- Cost of Python operations (`list.append` O(1), `x in list` O(n), `x in set` O(1))
- Frequency counting, seen-set, index map

**Python tools:** `set`, `dict`, `collections.Counter`, `collections.defaultdict`
**Problems:** Valid Anagram (LC 242) · Group Anagrams (LC 49) · Top K Frequent Elements (LC 347) · Product of Array Except Self (LC 238) · Longest Consecutive Sequence (LC 128)

## Session 2: Strings & Two Pointers
**Objectives:** manipulate strings efficiently, recognize two-pointer patterns.
- Strings are immutable: build with `"".join(list)`, not `+=` in a loop
- `ord` / `chr`, `isalnum`, `lower`, slicing `s[::-1]`
- Two pointers: opposite ends (sorted arrays, palindromes) and same direction (read/write pointers)

**Problems:** Valid Palindrome (LC 125) · Move Zeroes (LC 283) · Two Sum II (LC 167) · 3Sum (LC 15) · Container With Most Water (LC 11)

## Session 3: Sliding Window & Prefix Sums
**Objectives:** solve subarray/substring problems in O(n).
- Fixed-size window vs. variable-size window (expand right, shrink left)
- Prefix sums for range queries, prefix sum + hash map for subarray counting

**Problems:** Best Time to Buy and Sell Stock (LC 121) · Longest Substring Without Repeating Characters (LC 3) · Minimum Size Subarray Sum (LC 209) · Longest Repeating Character Replacement (LC 424) · Range Sum Query – Immutable (LC 303) · Subarray Sum Equals K (LC 560)

## Session 4: Sorting & Binary Search
**Objectives:** use sorting as a tool, master one reliable binary search template.
- Merge sort as an example of divide and conquer (O(n log n))
- Built-in sort: `sort(key=...)`, sorting tuples, stability
- Binary search template, lower / upper bound
- Binary search on the answer (monotonic condition)

**Python tools:** `sorted`, `list.sort(key=...)`, `bisect.bisect_left`, `bisect.bisect_right`
**Problems:** Binary Search (LC 704) · Search Insert Position (LC 35) · Merge Sorted Array (LC 88) · Find Minimum in Rotated Sorted Array (LC 153) · Search in Rotated Sorted Array (LC 33) · Koko Eating Bananas (LC 875)

## Session 5: Stacks, Queues & Linked Lists
**Objectives:** pick the right linear structure, handle pointer manipulation.
- Stack (LIFO) with `list`, queue (FIFO) with `deque`
- Monotonic stack (next greater element)
- Linked lists: dummy node, reversal, fast & slow pointers

**Python tools:** `list.append` / `list.pop`, `collections.deque`
**Problems:** Valid Parentheses (LC 20) · Min Stack (LC 155) · Daily Temperatures (LC 739) · Reverse Linked List (LC 206) · Merge Two Sorted Lists (LC 21) · Linked List Cycle (LC 141)

## Session 6: Recursion & Backtracking
**Objectives:** think recursively, generate all possibilities with backtracking.
- Base case, recursive case, call stack, recursion tree
- Complexity of recursive functions
- Backtracking template: choose → explore → un-choose
- Recursion limit: `sys.setrecursionlimit`

**Python tools:** `itertools.combinations`, `itertools.permutations` (to check answers)
**Problems:** Fibonacci Number (LC 509) · Pow(x, n) (LC 50) · Subsets (LC 78) · Permutations (LC 46) · Combination Sum (LC 39) · Word Search (LC 79)

## Session 7: Trees
**Objectives:** traverse trees with DFS and BFS, use BST properties.
- Binary tree terminology, `TreeNode` class
- DFS traversals: preorder, inorder, postorder (recursive)
- BFS level-order traversal with a queue
- Binary search tree: search, validation
- Bonus: Trie (prefix tree)

**Problems:** Maximum Depth of Binary Tree (LC 104) · Invert Binary Tree (LC 226) · Same Tree (LC 100) · Binary Tree Level Order Traversal (LC 102) · Validate Binary Search Tree (LC 98) · Diameter of Binary Tree (LC 543) · *Bonus:* Implement Trie (LC 208)

## Session 8: Heaps, Greedy & Intervals
**Objectives:** use a priority queue for top-K problems, recognize when greedy works.
- Heap operations and complexity; max-heap by negating values
- Top-K pattern
- Greedy: make the locally best choice, and justify why it is correct
- Intervals: sort by start, merge / count overlaps

**Python tools:** `heapq.heappush`, `heapq.heappop`, `heapq.heapify`, `heapq.nlargest`
**Problems:** Last Stone Weight (LC 1046) · Kth Largest Element in an Array (LC 215) · K Closest Points to Origin (LC 973) · Jump Game (LC 55) · Merge Intervals (LC 56) · Non-overlapping Intervals (LC 435)

## Session 9: Graphs I (Traversal)
**Objectives:** model problems as graphs, traverse them with BFS/DFS.
- Representations: adjacency list, grid as an implicit graph
- DFS and BFS, visited set, connected components
- BFS for shortest path in unweighted graphs (multi-source BFS)
- Topological sort (Kahn's algorithm), cycle detection

**Problems:** Flood Fill (LC 733) · Number of Islands (LC 200) · Clone Graph (LC 133) · Rotting Oranges (LC 994) · Course Schedule (LC 207) · Course Schedule II (LC 210)

## Session 10: Graphs II (Shortest Paths & Union-Find)
**Objectives:** handle weighted graphs and dynamic connectivity.
- Dijkstra with `heapq`
- Union-Find (path compression + union by rank)
- Bonus: minimum spanning tree (Kruskal with Union-Find)

**Problems:** Network Delay Time (LC 743) · Path With Minimum Effort (LC 1631) · Number of Provinces (LC 547) · Redundant Connection (LC 684) · *Bonus:* Min Cost to Connect All Points (LC 1584)

## Session 11: Dynamic Programming I (1D)
**Objectives:** go from recursion to memoization to tabulation.
- Overlapping subproblems and optimal substructure
- Steps: define the state → recurrence → base cases → order of computation
- Memoization (top-down) vs. tabulation (bottom-up), space optimization

**Python tools:** `functools.cache` / `functools.lru_cache`
**Problems:** Climbing Stairs (LC 70) · Min Cost Climbing Stairs (LC 746) · House Robber (LC 198) · Coin Change (LC 322) · Word Break (LC 139) · Longest Increasing Subsequence (LC 300)

## Session 12: Dynamic Programming II (2D)
**Objectives:** solve grid, two-sequence and knapsack DP.
- Grid DP
- Two-sequence DP (LCS, edit distance)
- 0/1 knapsack and subset sum

**Problems:** Unique Paths (LC 62) · Minimum Path Sum (LC 64) · Longest Common Subsequence (LC 1143) · Partition Equal Subset Sum (LC 416) · Edit Distance (LC 72)

## Session 13: Mock Interviews
**Objectives:** practise the full interview experience under time pressure.
- Members work in pairs (interviewer / candidate), 45 minutes per round, then swap
- Evaluation rubric: communication, problem solving, code quality, testing, complexity analysis
- Common mistakes recap and tips for the behavioral part

---

## Next: Contest Track (Python)
To be planned after the interview track:
- Fast I/O (`sys.stdin.readline`), PyPy on Codeforces, Python performance tips
- Math & number theory: gcd, sieve of Eratosthenes, modular arithmetic, fast exponentiation
- Bit manipulation: Single Number (LC 136), Counting Bits (LC 338), subsets with bitmasks
- Greedy & constructive problems
- Difference arrays, 2D prefix sums
- Fenwick tree / segment tree
- Advanced DP (bitmask DP, DP on trees)
- Weekly virtual contests + upsolving
