# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from a missing dependency in the `useEffect` call, leading to an infinite render loop.

## The Bug
The `bug.js` file contains a component with a `useEffect` hook that lacks the `count` variable as a dependency. This causes the effect to run on every render, triggering a continuous update cycle. 

## The Solution
The `bugSolution.js` file shows the corrected code. By adding `count` as a dependency to the `useEffect` hook, the effect only runs when the `count` variable changes, resolving the infinite loop.

## How to reproduce
1. Clone this repository.
2. Navigate to the repository folder in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the infinite loop in the console in the buggy version and the corrected behavior in the solution.