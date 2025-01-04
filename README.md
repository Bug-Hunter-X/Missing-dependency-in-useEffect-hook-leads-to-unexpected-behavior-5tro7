# React useEffect Hook Bug
This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug arises from a missing dependency in the `useEffect`'s dependency array, leading to unexpected behavior or even infinite loops.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders.  The dependency array determines when the effect should run. If a dependency is missing, the effect might run at unexpected times, leading to incorrect state updates or performance issues.

## Solution
The solution involves correctly identifying and including all the values that the effect relies on in the dependency array. In this case, the `count` variable should be listed in the dependency array.

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console log messages and the behavior of the counter.

## Learning
This example highlights the importance of paying close attention to the dependency array in `useEffect`. Missing dependencies is a source of subtle bugs that can be difficult to diagnose. Always carefully consider which variables your effect depends on.