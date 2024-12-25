# Expo Camera: undefined is not an object (evaluating 'cameraRef.current')

This repository demonstrates a common error when using the Expo Camera API and provides a solution. The error, "undefined is not an object (evaluating 'cameraRef.current')", arises from attempting to access the `cameraRef` before the camera component is fully mounted and initialized.

## The Problem
The problem lies in accessing `cameraRef.current` before Expo's Camera component is ready.  This usually happens within a `useEffect` hook where the code executes before the component's render cycle is complete.