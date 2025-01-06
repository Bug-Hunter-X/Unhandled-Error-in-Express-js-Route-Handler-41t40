# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers:  failure to handle cases where user input is invalid or missing.  Specifically, the provided code lacks proper error handling for non-numeric user IDs or IDs that don't match any existing user.

The `bug.js` file contains the problematic code. The `bugSolution.js` file shows the corrected version with proper error handling and more robust input validation.

## How to reproduce

1. Clone this repository.
2. Run `npm install express`
3. Run `node bug.js`
4. Send a request to `/users/abc` or `/users/1234` (assuming a user with that ID doesn't exist)