# Inconsistent Focus Styling Across Browsers

This repository demonstrates a common issue with the CSS `:focus-visible` pseudo-class and provides a solution for maintaining consistent styling across different browsers.

## Problem

The `:focus-visible` pseudo-class is designed to improve accessibility by only applying styles to elements when the focus is programmatically triggered. However, older browsers don't support this pseudo-class, leading to unexpected styling and potential usability problems.

The `bug.css` file showcases this issue.  In modern browsers, the outline will only appear when focusing using the keyboard.  Older browsers, however, will show the outline regardless of the focusing method.

## Solution

The `bugSolution.css` file provides a solution using JavaScript feature detection to conditionally apply the focus style.  This ensures consistency across browsers while maintaining accessibility best practices.

## Setup

1. Clone this repository.
2. Open `index.html` in your browser.
3. Test the focus behavior on different browsers (including older ones if possible).
