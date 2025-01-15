# React 19 useEffect Unexpected Behavior

This repository demonstrates an uncommon issue encountered in React 19 where the `useEffect` hook runs on every render, regardless of dependencies. This can lead to performance problems and unexpected behavior.  The solution demonstrates how to correctly specify dependencies to prevent this issue.

## Problem

The `bug.js` file showcases the problem: a `useEffect` hook logs a message on every render, even though it seems like there shouldn't be any dependencies. This is due to a subtle issue that might occur in some React 19 setups, possibly related to specific contexts or optimizations.

## Solution

The `bugSolution.js` file provides the corrected code.  The solution involves explicitly listing the dependencies to make the effect behave correctly and only run when necessary.  This demonstrates a proper use of the `useEffect` hook's dependency array. 