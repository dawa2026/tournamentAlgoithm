Project Description

This project implements the Tournament Sort algorithm in C++ to sort a list of integers in ascending order. The program does not use any built-in sorting functions.

    It also tracks:

The number of comparisons
The number of swaps (updates) performed during sorting

      How It Works

Tournament Sort works like a competition:

Elements are placed in the leaf nodes of a binary tree.
Each internal node stores the minimum of its two children.
The root node contains the smallest value.
That value is removed and replaced with a large value (INT_MAX).
The tree is updated to find the next smallest value.
This repeats until all elements are sorted.

       Example Execution

input:
4 2 7 1 3
Step-by-Step Process:
1.Initial tree built → Minimum = 1
2.Remove 1 → Update tree → Next minimum = 2
3.Remove 2 → Update tree → Next minimum = 3
4.Continue until sorted
Output:
Sorted array: 1 2 3 4 7
Comparisons: X
Updates: Y

Algorithm Analysis
Time complexity
-Best Case
O(n log n)Tree operations dominate

-Average Case
O(n log n)Balanced updates

-Worst Case
O(n²)Due to linear search for leaf

Space complexity
O(n)
-The tree array requires approximately 2 × n space

    Analysis of Results
-For small inputs, performance is fast
-For large inputs, performance slows due to:
-Linear search for minimum leaf
-Comparisons increase significantly with input size


    Improvements
-Store indices to avoid linear search → improves to O(n log n)
-Use Min Heap instead for efficiency
-Use dynamic arrays (vectors)

      Conclusion
This program of mine demonstrates how sorting algorithms work internally without relying on built-in functions. Tournament Sort provides a good understanding of tree-based selection but is less efficient than modern algorithms for large datasets.






       
