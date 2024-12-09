# Tailwind CSS: Silent Styling Failure Due to Invalid Class Names

This repository demonstrates a common yet subtle bug in Tailwind CSS:  the silent failure of applying styles when using misspelled or nonexistent class names.  The issue lies in the fact that Tailwind doesn't explicitly throw errors for invalid class names; it simply doesn't apply any styles associated with those names.

## The Bug

The `bug.js` file contains an example of how a misspelled class name can prevent a paragraph from being styled correctly, even though the rest of the styling works.  This can make debugging difficult as there are no immediate error messages indicating the problem.

## The Solution

The `bugSolution.js` file shows the corrected code, where the class names are used correctly. By correcting the typos and ensuring the class names are in the Tailwind configuration, styles are applied as expected.

## How to Reproduce

1. Clone this repository.
2. Run the `bug.js` file within a Tailwind project (ensure Tailwind is properly configured). Observe the unexpected styling.
3. Compare it with the correctly-styled output of `bugSolution.js` file.

This example helps illustrate the importance of carefully reviewing class names in your Tailwind projects and leveraging browser developer tools to quickly diagnose such errors.