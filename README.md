# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is designed to increment a numerical field by a specified value.  However, if you provide a string value instead of a number, the operation will fail.

## Bug
The `bug.js` file contains code that attempts to increment a counter field using a string value. This will result in an error.

## Solution
The `bugSolution.js` file demonstrates the correct way to use the `$inc` operator. It increments the counter field using a numerical value, ensuring the operation succeeds.

## How to reproduce the bug
1. Make sure you have MongoDB installed and running.
2. Create a collection named `myCollection` with a document containing a numerical field called `counter`.
3. Run the `bug.js` script. This will result in an error message.

## How to fix the bug
1. Replace the code in `bug.js` with the code from `bugSolution.js`.
2. Run the `bugSolution.js` script. This will successfully increment the counter field.