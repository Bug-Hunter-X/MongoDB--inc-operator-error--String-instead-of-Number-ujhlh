# MongoDB $inc Operator Error: String instead of Number

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numerical field in a document. However, if you provide a string value instead of a number, the update will fail or produce unexpected results.

## Bug
The `bug.js` file contains the erroneous code that uses a string ('1') as the increment value instead of a number (1).

## Solution
The `bugSolution.js` file demonstrates the correct way to use the `$inc` operator by passing a numerical value for incrementing the field.

## How to reproduce

1.  Make sure you have Node.js and a MongoDB instance running.
2.  Create a MongoDB collection.
3.  Run the code in `bug.js`. You'll see it doesn't work as expected or produces an error.
4.  Run the code in `bugSolution.js`.  This will correctly increment the field.