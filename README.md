# Merge Sort Algorithm (C++)

## Overview
This project implements the **Merge Sort algorithm** in C++. Merge Sort is a **divide-and-conquer sorting algorithm** that recursively divides an array into smaller subarrays, sorts them, and then merges them back together.

## Features
- User input-based array creation.
- Recursive merge sort implementation.
- Efficient sorting using divide and conquer technique.

## Algorithm Explanation
Merge Sort works in three main steps:
1. Divide the array into two halves.
2. Recursively sort both halves.
3. Merge the sorted halves into one sorted array.

## Functions

### merge(vector<int> &arr, int start, int mid, int end)
- Merges two sorted subarrays:
  - Left subarray → `start to mid`
  - Right subarray → `mid+1 to end`
- Uses a temporary vector to store sorted elements.

### mergeSort(vector<int> &arr, int start, int end)
- Recursively divides the array until single-element subarrays are formed.
- Calls `merge()` to combine sorted parts.

### show(const vector<int>& arr)
- Displays array elements.

## How to Compile and Run

### Compile
```bash
g++ main.cpp -o mergesort
Run
./mergesort
Example Input/Output
Input
Enter how many values you want to enter: 5
Enter #1: 8
Enter #2: 3
Enter #3: 10
Enter #4: 1
Enter #5: 7

Output
Before: 8 3 10 1 7
After: 1 3 7 8 10

Complexity
Time Complexity: O(n log n)
Space Complexity: O(n)

Concepts Covered
Divide and Conquer Algorithms
Recursion
Sorting Algorithms
Vector Manipulation

Possible Improvements
Add user choice for sorting order (ascending/descending).
Implement iterative merge sort.
Add performance benchmarking.

Author
Created for learning sorting algorithms in C++.
