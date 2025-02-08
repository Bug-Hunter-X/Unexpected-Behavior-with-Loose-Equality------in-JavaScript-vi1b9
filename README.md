# Unexpected Behavior with Loose Equality (==) in JavaScript

This repository demonstrates a common JavaScript bug caused by the loose equality operator (==).  Loose equality performs type coercion before comparison, which can lead to unexpected results.  The example shows how this can cause a function to produce incorrect output or throw an error.

## Bug Description

The `foo` function in `bug.js` uses loose equality (`==`) to check for null. This leads to unexpected behavior because loose equality may yield true when comparing different data types. For example 0 == false is true.  This can introduce subtle and hard-to-find bugs in applications.