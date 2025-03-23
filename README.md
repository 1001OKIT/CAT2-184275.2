# Big O Notation and Data Structures

## Overview
This repository contains an overview of Big O Notation and a comparison between Linked Lists and Arrays, along with sample code demonstrating these concepts.

## Big O Notation
Big O notation is used to describe the efficiency of an algorithm in terms of time and space complexity. The key rules include:

### 1. Ignoring Constants
Big O ignores constant multipliers. For example:
```
5n + 3 → O(n)
```

### 2. Removing Non-Dominant Terms
Only the term that grows fastest matters.
```
n² + n → O(n²)
```

### 3. Common Time Complexities
- **O(1)** - Constant time (e.g., accessing an array element)
- **O(log n)** - Logarithmic time (e.g., binary search)
- **O(n)** - Linear time (e.g., scanning an array)
- **O(n²)** - Quadratic time (e.g., nested loops)

### 4. Worst-Case vs Best-Case
Big O usually describes the worst-case scenario.
- Linear Search:
  - **Best case:** O(1) (element found at the first position)
  - **Worst case:** O(n) (element not found or at the last position)

### 5. Multiplication Rule
- **Consecutive loops** → Time complexities are added.
- **Nested loops** → Time complexities are multiplied.

Example:
```cpp
for(int i = 0; i < n; i++)  // O(n)
    for(int j = 0; j < n; j++)  // O(n)
        // Some operation
```
Overall complexity: **O(n²)**

---

## Linked Lists vs Arrays
### 1. Memory Allocation
- **Arrays:** Fixed contiguous memory allocation.
- **Linked Lists:** Dynamic memory allocation (non-contiguous).

### 2. Performance Comparison
| Operation       | Arrays | Linked Lists |
|----------------|--------|--------------|
| Access (by index) | O(1) | O(n) |
| Insertion (middle) | O(n) | O(1) (if node pointer is given) |

### Example: Array vs Linked List Insertion
- **Array:** To insert in the middle, elements must shift → **O(n)**.
- **Linked List:** If pointer to node is given → **O(1)**.

---

## How to Use the Code
1. Clone this repository:
   ```sh
   git clone https://github.com/your-repo.git
   ```
2. Navigate to the directory:
   ```sh
   cd your-repo
   ```
3. Compile and run the C++ examples:
   ```sh
   g++ big_o_examples.cpp -o big_o
   ./big_o
   ```

## License
This project is licensed under the MIT License.
