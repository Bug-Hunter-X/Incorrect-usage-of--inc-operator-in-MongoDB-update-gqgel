# Incorrect $inc Operator Usage in MongoDB Update
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The error arises from providing a string value instead of a numeric value to the `$inc` operator. This leads to unexpected results and potential data corruption.

## Bug
The `bug.js` file shows incorrect usage of `$inc`. The `count` field should be incremented by a numeric value; using a string results in the `$inc` operator failing to correctly increment the counter.

## Solution
The `bugSolution.js` file demonstrates the correct usage of `$inc`.  The solution involves ensuring a numerical value is passed to the `$inc` operator, guaranteeing correct update behavior.
