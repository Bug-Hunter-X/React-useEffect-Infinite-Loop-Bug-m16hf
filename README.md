# React UseEffect Infinite Loop Bug
This repository demonstrates a common React bug: an infinite loop caused by incorrect usage of the `useEffect` hook.  The `bug.js` file contains the buggy code, while `bugSolution.js` provides the corrected version.

## Bug Description
The bug arises from an infinite loop in the `useEffect` hook.  The state update within `useEffect` depends on the state that it is updating and this update is happening without proper dependency array. This leads to continuous re-renders, each triggering a new state update, resulting in an infinite loop. 

## Solution
The solution involves correctly managing the dependencies in `useEffect` hook.  The `bugSolution.js` demonstrates the correct use of dependency array to prevent this loop.