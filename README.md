# Longest Consecutive Sequence (Brute Force)

## Problem Statement

Given an unsorted array of integers, find the length of the longest sequence of consecutive elements. The consecutive numbers can appear in any order within the array.

## Approach

This solution uses the **Brute Force** approach.

For every element in the array:

* Treat it as the starting number of a sequence.
* Search the entire array to check whether the next consecutive number (`current + 1`) exists.
* If found, continue searching for the next consecutive number.
* Count the length of the sequence.
* Update the maximum sequence length found.

## Algorithm

1. Read the input array.
2. If the array is empty, return `0`.
3. For each element:

   * Initialize the current number and sequence length.
   * Repeatedly search the array for the next consecutive number.
   * Stop when the next number is not found.
4. Store the maximum sequence length.
5. Print the answer.

## Pattern Used

* Brute Force
* Linear Search

## Time Complexity

* **O(n²)**

## Space Complexity

* **O(1)**

## Notes

* This approach is easy to understand and useful for learning.
* It does **not** satisfy the `O(n)` time complexity required by LeetCode.
* The optimal solution uses a **HashSet** to achieve **O(n)** time complexity.
