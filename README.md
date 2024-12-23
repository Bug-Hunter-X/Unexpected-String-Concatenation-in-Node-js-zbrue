# Unexpected String Concatenation in Node.js

This example demonstrates a common but subtle error in JavaScript that occurs when performing arithmetic operations with values of mixed types. If one of the operands is a string, the `+` operator performs string concatenation rather than numerical addition.

The `bug.js` file showcases the issue. The `bugSolution.js` file provides a solution. 

## How to Reproduce
1. Save the code from `bug.js` into a file.
2. Run the file using Node.js: `node bug.js`
3. Observe the unexpected output.

## Solution
The solution is to ensure both operands are numbers before performing arithmetic operations.  The `bugSolution.js` demonstrates this using the `Number()` function.