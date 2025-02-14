# JavaScript Function Bug: Incorrect Null Handling

This repository demonstrates a common yet subtle bug in JavaScript functions related to the handling of null values. The `foo` function is designed to add two numbers, however it incorrectly returns 0 when either input is null. This can lead to unexpected behavior and incorrect results in applications.  The solution addresses this issue by correctly distinguishing between null and 0 values.

## Bug Description
The `foo` function returns 0 if either of its input parameters `a` or `b` is null.  It incorrectly treats null as equivalent to the numeric value 0. The expected behavior is to either return NaN (Not a Number) or handle the null values more appropriately depending on the specific use case. 

## Solution
The solution clarifies the handling of null values. Instead of simply returning 0, the updated function checks for null values explicitly and returns NaN if either input is null, which is a more appropriate response to invalid numeric inputs.