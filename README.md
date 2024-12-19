# Incorrect $inc usage in MongoDB Aggregation

This repository demonstrates a common error when using the `$inc` operator within a MongoDB aggregation pipeline's `$project` stage.  The `$inc` operator is intended for updating existing fields in documents, not for creating or modifying fields in the aggregation pipeline's projection stage.  The provided code shows the incorrect usage and a corrected version for proper aggregation.

## How to Reproduce the Bug
1. Clone this repository.
2. Run the provided MongoDB aggregation pipeline script (`bug.js`).
3. Observe the unexpected result of the `incorrectIncrement` field.

## Solution
The solution shows how to correctly achieve the intended result of incrementing the `count` value without the erroneous use of `$inc`.  The corrected script avoids the error and produces the expected output.