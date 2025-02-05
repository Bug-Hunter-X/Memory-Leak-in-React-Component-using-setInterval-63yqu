# React UseEffect Cleanup Function Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook and the `setInterval` function.  The bug showcases a memory leak caused by forgetting to provide a cleanup function within the `useEffect` hook.

## Problem
The `setInterval` function, when used within a React component's `useEffect` hook, requires a cleanup function to prevent memory leaks.  Failure to provide this cleanup function can lead to the interval continuing even after the component has unmounted.