# React useEffect Hook - Infinite Rendering Bug

This repository demonstrates a common bug related to the `useEffect` hook in React.  The component renders infinitely due to an issue with the dependency array.

## Bug Description
The `useEffect` hook is used to perform side effects after every render. However, if the dependency array is not correctly specified, it can lead to infinite rendering loops. In this example, the absence of `count` in the dependency array causes the effect to re-run on every render, triggering a never-ending cycle.

## Solution
The solution involves adding the `count` variable to the dependency array. This ensures that the effect only runs when the `count` value changes.

## How to Reproduce
1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the infinite rendering in the console.

## How to fix
Examine the corrected `bugSolution.js` for the solution which involves adding `count` to the dependency array of `useEffect`.
