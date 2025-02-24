# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  lack of error handling when parsing user input.  Specifically, the provided code attempts to parse a user ID as an integer without checking if the input is valid. This can lead to unexpected behavior or crashes if the ID is not a number.

## Bug

The `bug.js` file contains the erroneous code.  It attempts to find a user based on their ID, but doesn't handle the case where the ID is not a valid integer, or a user with that ID doesn't exist.

## Solution

The `bugSolution.js` file provides a corrected version of the code.  It includes error handling to check if the user ID is a valid integer and to handle the case where a user with the given ID is not found.