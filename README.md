# React useEffect Hook Missing Dependency

This repository demonstrates a common bug in React applications involving the `useEffect` hook: a missing dependency in the dependency array.  This can lead to unexpected behavior and difficult-to-debug issues.

## The Problem

The `bug.js` file contains a component that uses `useEffect` to log the current count. However, the `count` variable is missing from the dependency array. This means the effect only runs once after the initial render, even though the count changes on every click.

## The Solution

The `bugSolution.js` file shows the corrected component.  Adding `count` to the dependency array ensures that the effect runs every time the `count` variable changes.