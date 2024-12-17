# MongoDB $inc Operator with String Value
This repository demonstrates an uncommon error in MongoDB when using the `$inc` operator with a string value instead of a number.  The `$inc` operator is used to increment a numeric field by a specified value.  If a string is provided, the operation may fail silently or yield an unintended outcome.

## Bug
The `bug.js` file shows an incorrect use of `$inc` where a string ('10') is supplied.  This causes the operation to fail unexpectedly.

## Solution
The `bugSolution.js` file corrects the issue by using a numeric value (10) with the `$inc` operator.

## How to Reproduce
1.  Clone the repository.
2.  Ensure you have MongoDB running.
3.  Run `bug.js`. You'll observe the error.
4.  Run `bugSolution.js`. You'll see the correct incrementation.