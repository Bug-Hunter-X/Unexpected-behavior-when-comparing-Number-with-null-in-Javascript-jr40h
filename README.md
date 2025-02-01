# Unexpected behavior when comparing Number with null in Javascript
This code demonstrates an unexpected behavior when comparing a Number with null in Javascript. The issue arises in the conditional statements, particularly when comparing with zero. In JavaScript, the loose equality operator (==) does not distinguish between null and 0, causing the code to return 1 instead of 0 when 0 is provided as input. This behavior might not align with the intended logic. The solution involves using the strict equality operator (===) to explicitly distinguish between null, 0, and other numbers.

## How to reproduce the bug
1. Clone this repository.
2. Open `bug.js` and examine the code.
3. Run the code using a JavaScript interpreter.
4. Observe that when the input is 0, the output is 1 instead of 0. 

## Solution
The solution involves using the strict equality operator (===) instead of the loose equality operator (==) to distinguish between null and 0. This ensures that the code behaves as intended, returning 0 for null, -1 for negative numbers, and 1 for non-negative numbers.