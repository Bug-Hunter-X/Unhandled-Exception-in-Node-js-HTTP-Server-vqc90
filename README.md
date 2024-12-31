# Node.js Unhandled Exception Bug

This repository demonstrates a common error in Node.js: unhandled exceptions within an HTTP server.  The `bug.js` file shows a server that crashes when the `/error` route is accessed.  The `bugSolution.js` file provides a corrected version with proper error handling.

## Bug

The original code lacks a `try...catch` block to handle potential errors during request processing.  This leads to the server crashing and exiting unexpectedly. 

## Solution

The solution includes a `try...catch` block within the request handler to gracefully catch and handle exceptions.  This prevents the server from crashing and allows for more robust error management.
