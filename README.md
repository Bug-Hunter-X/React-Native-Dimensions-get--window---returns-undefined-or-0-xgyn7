# React Native Dimensions.get('window') Returns Undefined or Zero

This repository demonstrates a common issue in React Native development where `Dimensions.get('window')` returns `undefined` or an object with `width` and `height` set to 0. This can cause layout problems and crashes in your app.  The solution provided handles this situation gracefully.

## Problem
The `Dimensions` API, while useful for getting screen dimensions, can sometimes return unexpected values, especially during the initial render or rapid orientation changes.  Directly using the returned values without checking for validity can lead to errors.

## Solution
The solution uses conditional rendering to handle cases where `width` and `height` are undefined or zero.  A default size is used until valid dimensions are available.