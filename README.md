# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from an incomplete dependency array, leading to an infinite re-rendering loop.

## Problem
The `useEffect` hook is used to perform side effects after rendering. When the dependency array is missing or incomplete, the effect runs on every render, creating an infinite loop.  In this specific example, updating `count` triggers a re-render, which in turn triggers the effect again. The console will show this repeating.