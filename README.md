# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over an array.  The error occurs because the loop condition `i <= arr.length` tries to access an index beyond the array bounds, causing an `ArrayIndexOutOfBoundsException`.

The `bug.java` file contains the erroneous code. The `bugSolution.java` file provides the corrected code.

## How to reproduce the error

1. Compile and run `bug.java`.
2. Observe the `ArrayIndexOutOfBoundsException`. 

## Solution

The solution involves modifying the loop condition to `i < arr.length`, ensuring that the loop stops before attempting to access an index that is out of bounds.