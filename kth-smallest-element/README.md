Kth Smallest Element in an Array - C++ Solution
This repository contains a C++ solution to the problem of finding the kth smallest element in an array. The solution leverages a min-heap (priority queue) to efficiently find the desired element.

Problem Overview
Given an array of integers and an integer k, the task is to determine the kth smallest element in the array. This solution uses a min-heap to handle the problem with optimized time and space complexity.

Key Features
Efficient: The solution uses a priority queue (min-heap) to ensure that we can quickly find the kth smallest element.

Time Complexity: The algorithm runs in O(n log n) time, where n is the size of the array.

Space Complexity: The solution requires O(n) space due to storing elements in the heap.

Approach
Min-Heap: A priority queue is used to store elements in ascending order.

Heap Operations: By pushing all elements into the heap, the smallest elements are automatically ordered. We then pop elements from the heap k-1 times to reach the kth smallest element, which is left at the top of the heap.

Example Input/Output
Input: [12, 3, 5, 7, 19], k = 4

Output: The 4th smallest element is 12.
