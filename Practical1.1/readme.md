# DAA Practical 1.1 - Binary Search Algorithm

## Overview
This practical demonstrates the **Binary Search** algorithm, a fundamental Divide & Conquer searching technique implemented in three programming languages:
- Python
- Java
- C

## Binary Search Algorithm

### What is Binary Search?
Binary Search is an efficient algorithm for finding an element in a **sorted array**. It works by repeatedly dividing the search interval in half.

### Algorithm Steps:
1. Compare the target element with the middle element of the array
2. If the target matches the middle element, return its index
3. If the target is less than the middle element, search in the left half
4. If the target is greater than the middle element, search in the right half
5. Repeat until the element is found or the interval is empty

### Time Complexity:
| Case | Complexity |
|------|------------|
| Best | O(1) |
| Average | O(log n) |
| Worst | O(log n) |

### Space Complexity: O(1) (iterative approach)

## Files

| File | Description |
|------|-------------|
| `1.1Pracitcal.py` | Python implementation of Binary Search |
| `1.1 Practical.java` | Java implementation of Binary Search |
| `1.1Practical.c` | C implementation of Binary Search |
| `Practical 1.1.pdf` | Practical assignment document |

## Running the Code

### Python
```bash
python 1.1Pracitcal.py
```

### Java
```bash
javac 1.1 Practical.java
java BinarySearch
```

### C
```bash
gcc 1.1Practical.c -o 1.1Practical
./1.1Practical
```

## Example Output

**Python/Java:**
```
Enter number of elements: 5
Enter 5 sorted elements:
10
20
30
40
50
Enter element to search: 40
Element found at index: 3
```

**C:**
```
Element found at index 3
```

## Key Features
- ✅ Takes user input for array size and elements
- ✅ Accepts custom search key from user
- ✅ Returns index if element is found
- ✅ Returns -1 if element is not found
- ✅ Demonstrates iterative approach (no recursion overhead)

## Algorithm Flow
```
Start
  ↓
Set low = 0, high = n-1
  ↓
While low ≤ high:
  ↓
  Calculate mid = (low + high) / 2
  ↓
  If arr[mid] == key → Return mid
  ↓
  Else If key < arr[mid] → high = mid - 1
  ↓
  Else → low = mid + 1
  ↓
If element not found → Return -1
End
```

## Advantages of Binary Search
1. **Efficient**: O(log n) time complexity
2. **Simple**: Easy to understand and implement
3. **No Extra Space**: Constant space complexity
4. **Fast Search**: Much faster than linear search for large datasets

## Requirements
- Python 3.x
- Java JDK 8+
- GCC Compiler (for C)

## Subject
**Design and Analysis of Algorithms (DAA)**

---

*This practical is part of the DAA curriculum demonstrating fundamental searching algorithms.*

