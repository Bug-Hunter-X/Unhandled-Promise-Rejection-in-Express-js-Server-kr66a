# Unhandled Promise Rejection in Express.js Server

This repository demonstrates a common error in Express.js applications: unhandled promise rejections.  Asynchronous operations within route handlers can throw errors that crash the server if not properly handled.

The `bug.js` file shows an Express server with an asynchronous operation that rejects a promise.  The server lacks error handling, leading to a crash when the promise rejects.

The `bugSolution.js` file provides a solution by properly catching the error using `.catch()` and providing appropriate error responses to the client or logging the error effectively.