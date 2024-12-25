# React Component State Not Updating on Prop Changes

This repository demonstrates a common React bug where a component's state does not update correctly when props change. The issue is caused by using the wrong lifecycle method (`componentDidMount` instead of `componentDidUpdate`) for handling prop updates.

## Bug

The `MyComponent` component in `bug.js` demonstrates the bug. The state `count` should update whenever the `value` prop changes, but it only updates when the component initially mounts.

## Solution

The solution, shown in `bugSolution.js`, uses the `componentDidUpdate` lifecycle method to correctly update the state whenever the props change.

## How to run

1. Clone this repository
2. Navigate to the repository's directory
3. Run `npm install`
4. Run `npm start`