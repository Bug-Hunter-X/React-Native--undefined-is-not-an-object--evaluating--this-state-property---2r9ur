# React Native: undefined is not an object (evaluating 'this.state.property')

This repository demonstrates a common error in React Native where attempting to access component state or props before the component has mounted results in an 'undefined is not an object' error.  The solution utilizes the useEffect hook for proper state access after mounting.

## Problem

The `bug.js` file illustrates the problem.  Trying to access `this.state.count` within the `render` method before the component has a chance to initialize its state leads to the error.