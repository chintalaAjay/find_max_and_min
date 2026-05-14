# Find Minimum and Maximum Element in an Array - Java Solution

This repository contains my Java solution for the **Find Minimum and Maximum Element in an Array** problem from GeeksforGeeks.

---

## Problem Link

https://www.geeksforgeeks.org/problems/find-minimum-and-maximum-element-in-an-array4428/1

---

## Problem Statement

Given an array of integers, find the minimum and maximum elements present in the array.

The task is to return both the smallest and largest elements efficiently.

---

## Example

### Input

```text
[3, 2, 1, 56, 10000, 167]
```

### Output

```text
[1, 10000]
```

---

## Approach

### Linear Traversal Method

This approach uses a single traversal of the array.

### Steps

1. Initialize:
   - `max` with `Integer.MIN_VALUE`
   - `min` with `Integer.MAX_VALUE`

2. Traverse the array using a for-each loop.

3. Compare each element:
   - Update `max` if the current element is greater.
   - Update `min` if the current element is smaller.

4. Store the results inside an `ArrayList`.

This solution is efficient because both minimum and maximum are found in a single pass.

---

## Java Solution

```java
import java.util.ArrayList;

class Solution {
    public ArrayList<Integer> getMinMax(int[] arr) {

        ArrayList<Integer> list = new ArrayList<>();

        int max = Integer.MIN_VALUE;
        int min = Integer.MAX_VALUE;

        for (int i : arr) {

            if (i > max) {
                max = i;
            }

            if (i < min) {
                min = i;
            }
        }

        list.add(min);
        list.add(max);

        return list;
    }
}
```

---

## Time Complexity

```text
O(n)
```

The array is traversed only once.

---

## Space Complexity

```text
O(1)
```

Only a few extra variables are used.

---

## Concepts Used

- Arrays
- Array Traversal
- Minimum and Maximum Search
- ArrayList
- Time Complexity Optimization

---

## Learning Outcome

Through this problem, I learned:

- How to find minimum and maximum efficiently
- Using `Integer.MIN_VALUE` and `Integer.MAX_VALUE`
- Single-pass traversal optimization
- Returning values using `ArrayList`

---

## Author

Ajay Chintala

---

## GitHub Profile

https://github.com/chintalaAjay
