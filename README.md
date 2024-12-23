# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where a server can hang due to long-running requests blocking the event loop.  The `server.js` file showcases the problematic code. The `server-solution.js` file provides solutions using async/await and callbacks to address the blocking problem.

## Problem

The original code contains a long-running loop that blocks the event loop, preventing the server from handling subsequent requests. This leads to a hung server, unresponsive to any requests.

## Solution

The solution employs non-blocking techniques using either async/await or callbacks.  These methods prevent the event loop from being blocked, ensuring the server remains responsive.

## How to run

1. Clone the repository
2. Navigate to the project directory
3. Run `node server.js` (for the buggy version) or `node server-solution.js` (for the fixed version)