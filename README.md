# Unhandled 'undefined' in length property access

This repository demonstrates a common JavaScript error: failing to handle the 'undefined' case when accessing the 'length' property of an object.  The `bug.js` file contains the buggy code, and `bugSolution.js` provides a corrected version.

The issue occurs because the `foo` function attempts to access the `length` property of the input `x` without checking whether `x` is actually defined.  If `x` is `undefined`, a `TypeError` is thrown.

The solution involves explicitly checking for `undefined` before accessing `length`.