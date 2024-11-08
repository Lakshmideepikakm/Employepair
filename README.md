# Employepair
Here's a suitable question prompt you could use for your GitHub repository:

---

### Problem Statement: Employee Pairing Combinations

In a company, each employee can either:
- Work alone (remain single), or
- Form a pair with exactly one other employee.

Given an integer \( n \), which represents the total number of employees, write a program to find the number of ways to arrange them such that each employee is either working alone or paired with another. Note that:
- Pairing is symmetric, meaning that pairing (A, B) is the same as pairing (B, A).
- If \( n \) is odd, there will always be at least one single employee since they cannot all form pairs.
- If \( n \) is even, employees can all potentially be paired in various configurations.

The output should be the total number of possible configurations where employees can either pair up or remain single.

### Example Scenarios

1. **Example 1:**
   - **Input**: `n = 3`
   - **Output**: `4`
   - **Explanation**: The possible configurations are:
     - All singles: (A, B, C)
     - Pair (A, B), single (C)
     - Pair (A, C), single (B)
     - Pair (B, C), single (A)

2. **Example 2:**
   - **Input**: `n = 4`
   - **Output**: `10`
   - **Explanation**: The possible configurations are:
     - All singles: (A, B, C, D)
     - One pair and two singles:
       - Pair (A, B), singles (C, D)
       - Pair (A, C), singles (B, D)
       - Pair (A, D), singles (B, C)
       - Pair (B, C), singles (A, D)
       - Pair (B, D), singles (A, C)
       - Pair (C, D), singles (A, B)
     - Two pairs:
       - Pairs (A, B) and (C, D)
       - Pairs (A, C) and (B, D)
       - Pairs (A, D) and (B, C)

### Function Signature

```java
public static int countPairings(int n)
```

### Constraints

- \( 0 \leq n \leq 30 \)
  
Your solution should be efficient for large inputs, using dynamic programming or recursion with memoization to avoid recomputation.

### Additional Notes
This problem is a classic example of combinatorial arrangements and can be solved using recursive relations or dynamic programming techniques.
