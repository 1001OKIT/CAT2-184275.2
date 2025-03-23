
## 1. Big O Notation

Big O notation is used to describe the efficiency of algorithms, specifically their time and space complexity. [cite: 1]

### 1.1 Rules of Big O Notation

* **Ignore Constants:** Big O notation disregards constant factors. [cite: 2, 3] For example, O(5n + 3) simplifies to O(n). [cite: 3]
* **Remove Non-Dominant Terms:** Only the fastest-growing term is considered. [cite: 4, 5] For example, O(n² + n) simplifies to O(n²). [cite: 5]
* **Multiple Growth Rates:** Common time complexities include:
    * O(1) - Constant Time [cite: 6]
    * O(log n) - Logarithmic Time [cite: 6, 7, 8]
    * O(n) - Linear Time [cite: 6, 8, 9]
    * O(n²) - Quadratic Time [cite: 6, 9]
* **Worst-Case vs. Best-Case Analysis:** Big O typically describes the worst-case scenario. [cite: 10, 11, 12]
    * For example, in a linear search, the best-case time complexity is O(1), and the worst-case time complexity is O(n). [cite: 11, 12]
* **Multiplication Rule:**
    * Consecutive loops have complexities that are added.
    * Nested loops have complexities that are multiplied. [cite: 12]
    * Example:
        ```cpp
        for(int i = 0; i <= n; i++) // O(n)
        for(int j = 0; j < n; j++)  // O(n)
        ```
        The overall time complexity of the above code is O(n²). [cite: 12]

## 2. Linked Lists vs. Arrays

This section compares linked lists and arrays in terms of memory allocation and performance.

### Memory Allocation

* **Arrays:** Use fixed, contiguous memory allocation. [cite: 12]
* **Linked Lists:** Use non-contiguous, dynamic memory allocation. [cite: 12]

### Performance

* **Arrays:** Provide faster access to elements by index, with a time complexity of O(1). [cite: 12]
* **Linked Lists:** Have a time complexity of O(n) for element access because you have to traverse the list. [cite: 12]
* **Insertion**
    * **Arrays:** Insertion can be time-consuming, with a time complexity of O(n) in the middle of the array because elements have to be shifted. [cite: 12, 13]
    * **Linked Lists:** Insertion is efficient, with a time complexity of O(1) at the head if the node pointer is given. [cite: 12, 13]
