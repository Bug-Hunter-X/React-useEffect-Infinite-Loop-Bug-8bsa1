# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: creating an infinite loop within the `useEffect` hook.  The incorrect use of `setCount(count + 1)` inside the `useEffect` without proper dependency management leads to a continuous update cycle.

## Bug Description
The `useEffect` hook, when used without proper dependency management, can trigger an infinite loop. This occurs when the state update inside the `useEffect` causes the component to re-render, which, in turn, re-executes the `useEffect`, creating a never-ending cycle.  This example showcases this issue and its solution.

## Solution
The provided solution demonstrates the correct use of the `useEffect` hook.  Dependencies are properly handled to prevent the infinite loop.