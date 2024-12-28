# Unexpected Infinity in foo function when both inputs are 0

This repository demonstrates a common JavaScript error related to division by zero. The `foo` function does not correctly handle the case where both inputs are 0, leading to an unexpected `Infinity` result instead of 0 or NaN.

## Bug Description
The `foo` function is designed to return 0 if either input is 0, otherwise it returns the result of `a/b`. However, when both `a` and `b` are 0, the result is `Infinity`, which is incorrect. This happens because JavaScript does not throw an error on division by zero but returns `Infinity` instead.

## Solution
The solution addresses this issue by explicitly checking if both inputs are 0. If they are, the function returns 0 (or NaN, depending on the desired behavior). 

## How to run
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript editor. 
3. Run the code using Node.js or a browser console.

