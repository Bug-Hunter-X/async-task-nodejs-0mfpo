# Node.js Server Freeze: Synchronous Long-Running Task

This repository demonstrates a common issue in Node.js applications: server freezes caused by long-running synchronous operations within the request handler.  The `server.js` file contains a simple HTTP server with a computationally intensive loop that blocks the event loop, making the server unresponsive.

The solution (`serverSolution.js`) demonstrates how to address this by using asynchronous operations or offloading the task to a worker thread.