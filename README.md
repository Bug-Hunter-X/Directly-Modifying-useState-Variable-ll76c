# Directly Modifying useState Variable in React

This example demonstrates a common mistake when using React's `useState` hook: directly modifying the state variable instead of using the setter function. This can lead to unexpected behavior and prevent the component from re-rendering correctly.

## Bug
The `bug.js` file contains code that attempts to increment the `count` variable directly within a `useEffect` hook. This approach doesn't trigger a re-render because it doesn't update the state through the `setCount` function.

## Solution
The `bugSolution.js` file provides the corrected code, where the `count` variable is incremented using the `setCount` function, ensuring that the component re-renders and updates the UI accordingly.  This utilizes the functional update pattern for better state management.