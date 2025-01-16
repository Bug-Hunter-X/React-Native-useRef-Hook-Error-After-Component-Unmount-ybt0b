# React Native useRef Hook Error After Component Unmount

This repository demonstrates a common error in React Native applications involving the `useRef` hook and asynchronous operations.  When a component unmounts while an asynchronous operation (like a timer or a network request) is still in progress, attempting to access `ref.current` within that operation will result in errors because the component's instance no longer exists.

The `bug.js` file shows the problematic code, and `bugSolution.js` provides a corrected version.