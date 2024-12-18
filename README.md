# React Native FlatList Performance Issue

This repository demonstrates a common performance issue in React Native when using FlatList with very large datasets.  The initial render is extremely slow, causing noticeable UI freezes.

## Problem

The provided `bug.js` file contains a simple FlatList component rendering 10000 items.  On lower-end devices or emulators, the rendering time is significantly long, resulting in a poor user experience.

## Solution

The `bugSolution.js` file provides an optimized solution using techniques like `windowSize`, `initialNumToRender`, and potentially virtualization libraries for significantly improved performance.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npx react-native run-android` (or `npx react-native run-ios`).
4. Observe the slow rendering of the list in the `bug.js` example.
5. Compare the performance improvement in the `bugSolution.js` example.
