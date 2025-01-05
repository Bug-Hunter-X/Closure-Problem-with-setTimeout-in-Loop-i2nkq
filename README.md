# JavaScript Closure Problem with setTimeout in Loop

This repository demonstrates a common closure-related issue in JavaScript when using `setTimeout` within a loop.  The problem arises because the `setTimeout` callback function references the loop variable `i`, not its value at the time of the `setTimeout` call. By the time the `setTimeout` callbacks finally execute, the loop has already completed, and `i` will be its final value (10).

The `bug.js` file contains the code exhibiting the issue.  The `bugSolution.js` provides a corrected version.