# Express.js Route Parameter Error Handling

This repository demonstrates a common error in Express.js route handlers: failure to handle invalid or missing parameters.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version with robust error handling.

The error occurs when a non-numeric ID is passed to the `/users/:id` route. The code attempts to parse this using `parseInt`, but if the parsing fails it throws an error.  The solution introduces checks to prevent this and provides more graceful error handling for non-existent users.