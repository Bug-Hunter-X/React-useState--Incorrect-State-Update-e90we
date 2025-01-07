# React useState: Incorrect State Update

This repository demonstrates a common error when using the `useState` hook in React: directly modifying the state variable instead of using the setter function.  This leads to unexpected behavior where the UI does not update even though the state variable appears to change.

## Problem

The `bug.js` file shows the incorrect approach.  The `count` variable is directly modified using `count = count + 1;` which does not trigger a re-render in React. Only calling the `setCount` function updates the UI.

## Solution

The `bugSolution.js` file provides the correct solution.  The state is updated exclusively by calling `setCount(count + 1);` which triggers a re-render and reflects the change in the UI.

## How to run

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.