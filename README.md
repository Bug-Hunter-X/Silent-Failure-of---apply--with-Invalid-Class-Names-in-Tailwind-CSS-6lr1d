# Silent Failure of @apply with Invalid Class Names in Tailwind CSS

This repository demonstrates a subtle bug in Tailwind CSS when using the `@apply` directive with an invalid class name.  The issue is that Tailwind doesn't throw an error if the class name doesn't exist, it simply doesn't apply any styles. This makes debugging challenging, as the developer won't receive any error messages.

The `bug.html` file shows the incorrect usage of the `@apply` directive.  The `bugSolution.html` shows the solution. 

## Steps to Reproduce

1. Clone the repository
2. Open `bug.html` in your browser. You'll see that the `div` element doesn't have the expected styles.
3. Open `bugSolution.html` to see the correct implementation.

## Solution

The solution is to carefully check that the class names used with `@apply` exist in your Tailwind configuration. Utilize your IDE's autocompletion and linting features to catch these errors during development.