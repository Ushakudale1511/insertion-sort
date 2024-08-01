Insertion sort is a simple and intuitive sorting algorithm that works similarly to the way you might sort playing cards in your hands. It builds the final sorted array (or list) one item at a time. Here is a detailed explanation of how the insertion sort algorithm works:

**Steps of Insertion Sort**

1)Starting Point: Begin with the second element of the array, as the first element is trivially sorted.

2)Key Element: Consider the current element to be the key element. The goal is to insert this key element into its correct position in the already sorted part of the array.

3)Shifting Elements: Compare the key element with the elements before it (elements in the sorted portion). If the key element is smaller than the element it's compared with, shift that element one position to the right. Continue this process until you find the correct position for the key element.

4)Insertion: Insert the key element at its correct position.

5)Repeat: Move to the next element and repeat steps 2-4 until the entire array is sorted.

**Example**

Consider an array [12, 11, 13, 5, 6]. Here is how insertion sort will sort this array step by step:

Initial Array: [12, 11, 13, 5, 6]

First Iteration:

Key Element: 11
Compare 11 with 12 (the element before it).
Since 11 is smaller than 12, shift 12 to the right.
Insert 11 at the beginning.
Result: [11, 12, 13, 5, 6]

Second Iteration:

Key Element: 13
Compare 13 with 12 (the element before it).
Since 13 is greater than 12, it stays in its position.
Result: [11, 12, 13, 5, 6]
Third Iteration:
Key Element: 5
Compare 5 with 13, 12, and 11.
Since 5 is smaller than all of them, shift them all to the right.

Insert 5 at the beginning.

Result: [5, 11, 12, 13, 6]

Fourth Iteration:

Key Element: 6

Compare 6 with 13, 12, and 11.

Shift 13 and 12 to the right.

Insert 6 after 5.

Result: [5, 6, 11, 12, 13]
The array is now sorted.

Characteristics of Insertion Sort

**Time Complexity:**

**Worst-case: **

𝑂(𝑛2)

O(n 2) (when the array is sorted in reverse order).

**Best-case: 𝑂(𝑛)**

O(n) (when the array is already sorted).

**Average-case: **
𝑂(𝑛2)
O(n 2).

**Space Complexity: **
𝑂(1)

O(1) (in-place sorting).

**Stability:** Insertion sort is a stable sorting algorithm, meaning that it maintains the relative order of equal elements.

**Adaptive: **It is adaptive in nature, meaning that it is efficient for data sets that are already substantially sorted.
