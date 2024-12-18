# Java ArrayIndexOutOfBoundsException Bug

This repository demonstrates a common off-by-one error in Java that leads to an `ArrayIndexOutOfBoundsException`. The `BuggyArray.java` file contains the erroneous code, while `FixedArray.java` provides a corrected version.

The bug occurs in the `for` loop's condition, which should be `i < array.length` instead of `i <= array.length`.  The original code tries to access an element at index 5 in an array of size 5.  This causes the exception.

The fix is simple: changing the loop condition to `i < array.length` prevents access to the non-existent element at index 5. 