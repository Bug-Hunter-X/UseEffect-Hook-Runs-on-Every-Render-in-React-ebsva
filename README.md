# React useEffect Hook Runs on Every Render
This repository demonstrates a common mistake when using the `useEffect` hook in React. The effect runs on every render even when a dependency array is provided.

## Bug Description
The `useEffect` hook is intended to perform side effects after a component renders.  However, if the dependency array is not correctly specified or contains unnecessary dependencies, the effect might run more frequently than expected, leading to performance issues or unexpected behavior.

## Solution
The solution involves correctly specifying the dependency array to include only the variables that trigger the effect's execution. In this case, only the `count` state variable needs to be included.