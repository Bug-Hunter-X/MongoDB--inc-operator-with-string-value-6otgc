# MongoDB $inc operator with string value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided as the increment value, MongoDB will not correctly increment the field.

## Bug Description

The provided code attempts to increment the `age` field in a document by 1. However, the `$inc` value is provided as a string, which results in an error or unexpected behavior.

## Bug Solution

The correct approach is to provide a numeric value to the `$inc` operator. The solution provided in `bugSolution.js` demonstrates the correct usage.