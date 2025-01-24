# Uncommon HTML Bug: Handling Non-Existent Elements

This repository demonstrates a subtle bug related to accessing non-existent elements in HTML using JavaScript.  The bug arises when attempting to access an element that does not exist in the DOM using `document.querySelector`.

The solution involves adding checks to prevent errors and handle null values gracefully.

## Bug
The original HTML file (`bug.html`) attempts to access a paragraph element with the class `nonexistent`, which does not exist. This results in `null` being assigned to the `element` variable.  If code proceeds to use `element` without a null check, it can cause errors.

## Solution
The solution (`bugSolution.html`) addresses this by checking if `element` is null before attempting to use it.  This prevents errors from occurring.  The improved code gracefully handles cases where the targeted element is absent.
