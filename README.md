# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js servers: unresponsiveness due to long-running operations that block the event loop.  The example simulates a slow database query or other time-consuming task that causes the server to hang.

The `bug.js` file contains the problematic code, while `bugSolution.js` shows how to fix it using asynchronous programming.

## How to Reproduce

1. Clone the repository.
2. Navigate to the project directory.
3. Run `node bug.js`.
4. Open your browser and access `http://localhost:3000`.  Notice the delay.
5. Try making multiple requests simultaneously.  Observe the unresponsiveness.

## Solution

The solution in `bugSolution.js` showcases the proper use of asynchronous techniques (e.g., promises or async/await) to prevent blocking the event loop and maintain server responsiveness.