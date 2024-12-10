# Implicit Return Bug in JavaScript

This repository demonstrates a common error in JavaScript: the implicit return of `undefined` when a function's execution path doesn't explicitly reach a `return` statement.  This can lead to unexpected results and difficult-to-debug issues.

## The Bug

The `bug.js` file contains a function `foo` that checks for `null` values as input. However, it's missing an explicit `return` statement in the `if` block, making its behavior unpredictable when either `a` or `b` is `null`.

## The Solution

The `bugSolution.js` file provides the corrected version of the function, including an explicit `return null` statement for the case where null values are detected.