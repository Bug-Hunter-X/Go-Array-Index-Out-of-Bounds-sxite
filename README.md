# Go Array Index Out of Bounds Bug

This repository demonstrates a common error in Go: attempting to access an array index that is out of bounds.  The `bug.go` file contains the buggy code, which leads to a runtime panic. The `bugSolution.go` file shows the corrected code.

## Bug Description

The bug occurs because the loop in `main` iterates from 0 to 10 (inclusive), while the array `a` only has indices from 0 to 9.  When `i` reaches 10, accessing `a[i]` results in an index out of bounds error and a program crash.

## Solution

The solution is to change the loop condition to `i < 10`, ensuring that the loop stops before attempting to access an invalid index.