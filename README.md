# React Native Asynchronous Data Loading Bug

This repository demonstrates a common error in React Native applications: attempting to access properties of an object before it has been fully loaded from an asynchronous operation.  The bug is in `bug.js` and a solution is provided in `bugSolution.js`.

The error, "Cannot read properties of undefined (reading 'name')", arises when the component tries to render `data.name` while `data` is still null or undefined. This typically occurs with API calls or other asynchronous data fetching.

The solution involves using optional chaining or the nullish coalescing operator to safely access the property.