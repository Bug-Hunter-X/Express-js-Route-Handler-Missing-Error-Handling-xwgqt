# Express.js Route Handler Missing Error Handling

This example demonstrates a common error in Express.js route handlers: missing error handling for invalid or missing parameters.  The code attempts to access a user based on a provided ID, but lacks checks for invalid input or the absence of a user.

## Bug

The `bug.js` file shows a route handler that fetches a user by ID. If the ID is not a number, or no user with that ID exists, the code will crash or return an unexpected error. 

## Solution

The `bugSolution.js` file shows the improved route handler with added error handling. It checks if the ID is a number and if a user with that ID exists, returning appropriate error responses if either condition isn't met.