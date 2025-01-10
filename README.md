# Unexpected Calculation Results with calc() in CSS

This repository demonstrates a common issue when using the `calc()` function in CSS: unexpected results when the parent element's width is not explicitly set.  The `calc()` function is powerful but can be tricky if not used carefully.

## Bug Report

The `bug.css` file demonstrates the issue.  Notice how `calc(100% - 10px)` behaves unpredictably. 

## Solution

The `bugSolution.css` file provides a solution. It shows how to properly use `calc()` when there are potential issues with parent widths. Explicitly setting a width (or using viewport units) on the parent container ensures that `calc()` functions properly.