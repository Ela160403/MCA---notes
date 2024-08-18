#### Introduction to Arrays in Java 🚀

#### Day 1 - 19-08-2024

#### **📖 Concept of Arrays**

Arrays in Java are a collection of elements, all of the same type, stored in a contiguous memory location. They allow you to store multiple values in a single variable, making data management more efficient. Arrays are fixed in size and can be accessed using an index.


#### **Real time Example**
![Input](/images/Array.png)


#### **✨ Advantages of Arrays**

- ***Efficient Memory Usage***: Arrays store elements in contiguous memory locations, leading to efficient data retrieval.
- ***Ease of Access***: Elements can be accessed quickly using their index, making arrays ideal for scenarios requiring fast lookups.
- ***Data Management***: Store and manage large volumes of data in a structured format.
- ***Fixed Size***: Knowing the array size beforehand ensures better memory allocation and management.

#### **🌟 Use Cases of Arrays**

- ***Data Storage***: Store a list of elements, such as numbers or strings.
- ***Matrix Operations***: Represent matrices and perform mathematical operations on them.
- ***Sorting and Searching Algorithms***: Implement and optimize algorithms for data sorting and searching.
- ***Handling Multiple Variables***: Manage collections of similar data types, such as student grades or product prices.

#### **🛠️ Implementing Array Problems in Java**

***1. Peak Element Problem***

Given a 0-indexed array of integers `arr[]` of size `n`, find its peak element and return its index. An element is considered to be a peak if its value is greater than or equal to the values of its adjacent elements (if they exist).

***Constraints***:
- 1 ≤ n ≤ 10⁵
- 1 ≤ arr[i] ≤ 10⁶

***Expected Time Complexity***: O(log(n))
***Expected Auxiliary Space***: O(1)

***Example 1***:
```java
Input: n = 3, arr[] = {1, 2, 3}
Output: 1
Explanation: The index 2 with value 3 is a peak element since it's greater than its adjacent elements.
```

***Example 2***:
```java
Input: n = 7, arr[] = {1, 1, 1, 2, 1, 1, 1}
Output: 1
Explanation: In this case, multiple indices could be peak elements. Returning any of them is correct.
```

***Solve Here to Get Credits***: [GeeksforGeeks - Peak Element Problem](https://www.geeksforgeeks.org/problems/peak-element/1)

***2. Move Zeros Problem***

Given an integer array `nums`, move all 0's to the end of it while maintaining the relative order of the non-zero elements. This must be done in-place without making a copy of the array.

***Constraints***:
- 1 ≤ nums.length ≤ 10⁴
- -2³¹ ≤ nums[i] ≤ 2³¹ - 1

***Example 1***:
```java
Input: nums = [0,1,0,3,12]
Output: [1,3,12,0,0]
```

***Example 2***:
```java
Input: nums = [0]
Output: [0]
```

***Solve Here to Get Credits***: [LeetCode - Move Zeros Problem](https://leetcode.com/problems/move-zeroes/description/)

#### **❓ Array Questions to Practice**

1. ***Peak Elements***:
   - ***Objective***: Find and return the peak element in an array.
   - ***Key Concept***: Understanding array traversal and binary search.

2. ***Move Zeros***:
   - ***Objective***: Move all zeros to the end of the array without using an additional array.
   - ***Key Concept***: In-place array manipulation.

#### **📚 Suggested Reading**

- [Arrays: A Step-by-Step Guide for Concurrent Programming](https://www.geeksforgeeks.org/array-data-structure-guide/#types-of-array-data-structures)
