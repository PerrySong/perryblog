---
layout: post
title: "Binary Search"
date: 2018-08-27 
description: "Binary Search subtypes and templates"
tag: Algorithms
---   

# Binary Search  

Example: Given an sorted integer array - nums, and an integer - target.
Find the any/first/last position of target in nums Return -1 if target does not exist.
 
# Run time:   
  T(n) = T(n/2) + O(1) = O(logn)

# Implementation:
Recursion or While loop

# Binary Search code template:
1. start + 1 < end // While loop condition
2. start + (end - start) / 2 // Mid's value in case of number overflow.
3. A[mid] ==, <, > // Move pointers conditions
4. A[start] A[end] ? target //Check tail in the end
  
# Warm up question:
1. Find any position of a target number in a sorted array. Return -1 if target does not exist.

2. For a given sorted array (ascending order) and a target number, find the first index of this number in O(log n) time complexity. If the target number does not exist in the array, return -1.

# Binary Search Questions Subtypes:
1. OO/XX Find the first/last element in an array that statisfied some condition.  
   Examples : Bad Version, Search In a Big Sorted Array,  Find Minimum in Rotated Sorted Array  

2. Can not find a certain condition to find sepcific element but can retain the half which has the result or abandon the half that we know does not have the result.    
Examples: Find Peak Element, Search in Rotated Sorted Array

3. Binary Search on Result: There is no array for binary search but we are looking for some result that fit the conditions.  

   Examples: Sqrt(x), Wood Cut, Copy Books
