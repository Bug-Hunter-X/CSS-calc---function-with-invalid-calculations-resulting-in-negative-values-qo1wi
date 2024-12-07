# CSS calc() function with invalid calculations resulting in negative values

This repository demonstrates an uncommon bug related to the CSS `calc()` function.  When `calc()` results in a negative value, which is invalid for many CSS length properties, unexpected behavior may occur. This example shows how subtracting a larger value from a smaller value leads to unpredictable layout issues.

The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution using `max()` or `min()` to ensure valid CSS length values.  This is a simple yet important edge case to be aware of when working with dynamic CSS calculations.