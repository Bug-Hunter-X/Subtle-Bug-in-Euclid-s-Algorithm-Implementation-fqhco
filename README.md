# Subtle Bug in Euclid's Algorithm JavaScript Implementation

This repository demonstrates a subtle bug in a JavaScript implementation of Euclid's algorithm for finding the greatest common divisor (GCD).  The code appears to work correctly for many inputs, but fails under specific conditions.

## Bug Description
The `myFunction` function correctly calculates the GCD for most positive integer pairs. However, it produces unexpected results when dealing with negative numbers. The issue stems from the use of `Math.abs` within the recursive call which handles the subtraction logic incorrectly in certain scenarios involving negative numbers.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run the code using a Node.js environment (e.g., `node bug.js`).
4. Observe the output and note any unexpected results when negative inputs are used.

## Solution
The solution involves modifying the recursive call to handle negative numbers more robustly.  See `bugSolution.js` for the corrected implementation. This revised version ensures the proper handling of negative numbers, thereby providing a more comprehensive and accurate GCD calculation.
