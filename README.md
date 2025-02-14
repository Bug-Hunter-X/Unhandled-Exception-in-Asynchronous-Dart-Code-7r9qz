# Unhandled Exception in Asynchronous Dart Code

This repository demonstrates a common error in Dart asynchronous programming where exceptions are caught but not properly propagated.  The example shows how to use `rethrow` effectively.

## Bug Description:
The `fetchData` function fetches data from a remote API.  While it handles exceptions within the `catch` block, it fails to rethrow the exception, preventing higher-level error handling.

## Solution:
Adding `rethrow` ensures that the exception is propagated up the call stack, allowing for more robust error handling in the calling function.
