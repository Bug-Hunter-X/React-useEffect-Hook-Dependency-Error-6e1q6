# React useEffect Hook Dependency Error

This repository demonstrates a common error in React's `useEffect` hook where a dependency is missing from the dependency array, leading to an infinite render loop.  The `bug.js` file shows the incorrect code, while `bugSolution.js` provides the correct implementation.

The error occurs because the effect function is called after every render. Correctly specifying the dependency array prevents unnecessary re-renders and resolves the issue.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the infinite rendering in the console and browser.

## Solution

The solution is to add the `count` variable to the dependency array of the `useEffect` hook. This ensures that the effect only runs when the `count` variable changes. 