# Unexpected Null Return in Addition Function

This repository demonstrates a common JavaScript error: unexpected null return values when null values are passed as function arguments.

The `foo` function is intended to add two numbers.  However, it currently returns `null` if either input is `null`. A more robust solution would handle null values more gracefully, perhaps by treating them as 0.

## Bug

The bug is present in `bug.js`. The function immediately returns `null` when encountering a null value, instead of handling the null as a 0 value for summation.

## Solution

The solution is provided in `bugSolution.js`.  The function now explicitly checks for null values and treats them as 0 before performing the addition.