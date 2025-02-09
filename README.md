# Uncommon HTML Error: getAttribute() vs. Property Access

This repository demonstrates a subtle difference in how JavaScript handles accessing non-existent attributes versus non-existent properties on HTML elements.  Attempting to get a non-existent attribute using `getAttribute()` silently returns `null`, while trying to directly access a non-existent property throws a `TypeError`.

## Bug Description
The `bug.html` file contains JavaScript code that attempts to access a non-existent attribute and a non-existent property of an HTML element. The difference in the outcome is shown in the browser's console.

## Solution
The `solution.html` file shows how to handle non-existent attributes gracefully while mitigating the risk of unexpected errors caused by accessing non-existent properties. Always check for `null` when using `getAttribute()` for expected values.