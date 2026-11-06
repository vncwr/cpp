# C++ Practice Problems

This document describes the problems represented by the exercises in this
repository. They are grouped from introductory to more challenging. Each
problem is independent and can be solved using the corresponding source file
as a starting point.

## Easy

### 1. Reverse a String and an Array

Given a string and an integer array, reverse both sequences in place.

**Example**

```text
Input:  string = "hello", array = [2, 4, 23, 5]
Output: string = "olleh", array = [5, 23, 4, 2]
```

Related file: `STL/algorithm/reverse.cpp`

### 2. Sort Values in Ascending and Descending Order

Given an integer array and an integer vector, sort the array in ascending
order and the vector in descending order.

**Example**

```text
Input:  array = [1, 34, 6, 3], vector = [1, 4, 235, 3]
Output: array = [1, 3, 6, 34], vector = [235, 4, 3, 1]
```

Related file: `STL/algorithm/sort.cpp`

### 3. Calculate Array Aggregates

For an integer array, calculate:

1. Whether a target value exists.
2. The number of even values.
3. The sum of all values.
4. The product of all values.

**Example**

```text
Input:  [2, 4, 23, 5], target = 4
Output: exists = true, even_count = 2, sum = 34, product = 920
```

Related file: `STL/algorithm/search.cpp`

### 4. Find the Digital Root

Given a non-negative integer, repeatedly add its digits until only one digit
remains. Return that digit.

**Example**

```text
Input:  9875
Output: 2
```

Related function: `sumOfDigs` in `dcsdays.cpp`

### 5. List Odd Numbers in an Interval

Given two bounds `a` and `b`, return every odd integer in the inclusive
interval `[a, b]`.

**Example**

```text
Input:  a = 3, b = 10
Output: [3, 5, 7, 9]
```

Related function: `oddNumIR` in `dcsdays.cpp`

### 6. Check Whether a String Is a Palindrome

Determine whether a string reads identically from left to right and from right
to left.

**Example**

```text
Input:  "level"
Output: true
```

Related function: `isPalindrome` in `dcsdays.cpp`

### 7. Count Character Frequencies

Given a string, count how many times each character occurs.

**Example**

```text
Input:  "banana"
Output: b: 1, a: 3, n: 2
```

Related function: `freqCounter` in `dcsdays.cpp`

### 8. Find the Minimum and Maximum

Given a non-empty integer array, return its minimum and maximum values.

**Example**

```text
Input:  [7, 2, 9, 4]
Output: minimum = 2, maximum = 9
```

Related function: `minMax` in `dcsdays.cpp`

### 9. Basic Singly Linked-List Operations

Implement a singly linked list supporting:

- Inserting a node at the front.
- Inserting a node at the back.
- Inserting a node at a one-based position.
- Deleting a node at a one-based position.
- Counting nodes.
- Printing all values.

**Example**

```text
Operations: insert_back(10), insert_front(5), insert(2, 7), delete(1)
Output:     [7, 10]
```

Related file: `node.cpp`

## Medium

### 10. Two Sum

Given an integer array and a target value, return the indices of two distinct
elements whose values add up to the target. Return an empty result if no such
pair exists.

**Example**

```text
Input:  nums = [2, 7, 11, 15], target = 9
Output: [0, 1]
```

Related functions: `twoSum` in `strings.cpp` and the demonstration in
`dcsdays.cpp`

### 11. Sort Odd and Even Values by Different Rules

Rearrange an integer array so that:

1. Odd values appear first in descending order.
2. Even values appear afterward in ascending order.

**Example**

```text
Input:  [5, 2, 9, 4, 7, 6]
Output: [9, 7, 5, 2, 4, 6]
```

Related function: `customSort` in `dcsdays.cpp`

### 12. Find the K-th Largest Element

Given an integer array and an integer `k`, return the `k`-th largest value.
Equal values occupy separate positions.

**Example**

```text
Input:  nums = [3, 2, 1, 5, 6, 4], k = 2
Output: 5
```

Related function: `kthLE` in `dcsdays.cpp`

### 13. Find the Longest Common Prefix

Given a list of strings, return the longest prefix shared by every string.
Return an empty string when no common prefix exists.

**Example**

```text
Input:  ["flower", "flow", "flight"]
Output: "fl"
```

Related function: `longestCommonPrefix` in `strings.cpp`

### 14. Implement Bubble Sort and Selection Sort

Implement bubble sort and selection sort for an integer vector. Both functions
must sort the vector in non-decreasing order.

**Example**

```text
Input:  [5, 1, 4, 2, 8]
Output: [1, 2, 4, 5, 8]
```

Related file: `sorting.cpp`

### 15. Reverse Only Non-Letter Characters

Given a string containing letters and non-letter characters, keep every letter
in its original position while reversing the order of all non-letter
characters.

**Example**

```text
Input:  "a-bc-d"
Output: "a-dc-b"
```

Related function: `SRC` in `dcsdays.cpp`

### 16. Work with a Doubly Linked Node

Create a doubly linked structure in which each node stores a value, a pointer
to the previous node, and a pointer to the next node. Build a three-node list
and retrieve the value of the previous node from the last node.

**Example**

```text
Input:  1 <-> 2 <-> 3
Output: 2
```

Related class: `Node` in `node.cpp`

### 17. Return a Pointer to a Vector Element

Given a vector and a valid index, return a pointer to the element at that
index. Use the pointer to read or modify the original element.

**Example**

```text
Input:  values = ["hello", "world"], index = 0
Output: "hello"
```

Related functions: `getP` and `getSP` in `pointers.cpp`

## Hard

### 18. Median of Two Sorted Arrays

Given two sorted integer arrays, find the median of the combined values.
The result may be fractional.

**Example**

```text
Input:  [1, 3], [2]
Output: 2.0
```

Related function: `findMedianSortedArrays` in `strings.cpp`

### 19. Container With the Most Water

Given an array where `height[i]` represents the height of a vertical line at
position `i`, choose two lines that form a container holding the maximum
possible amount of water. Return the maximum area.

**Example**

```text
Input:  [1, 8, 6, 2, 5, 4, 8, 3, 7]
Output: 49
```

Related function: `maxArea` in `strings.cpp`

### 20. Binary Search in a Sorted Array

Given a sorted array and a target value, use binary search to find the target.
Return its index, or `-1` if it is absent.

**Example**

```text
Input:  values = [1, 3, 5, 7, 9], target = 7
Output: 3
```

Related demonstration: `strings.cpp`

## Notes

The source files are learning exercises and demonstrations, so some functions
do not yet handle every boundary case. The problem statements above define the
intended behavior and can be used as specifications for improving the
implementations.
