# CSS Specificity Gotcha: Unexpected Color Inheritance

This repository demonstrates a subtle but important issue related to CSS selector specificity.  The bug involves unexpected color inheritance due to the order and specificity of CSS selectors.

## The Problem

The `bug.css` file contains CSS rules that unexpectedly result in the text color being red, even though it seems like it should be blue based on a naive understanding of selector precedence.

## The Solution

The `bugSolution.css` file shows how to resolve the issue and provides a clear explanation of why the original code behaved incorrectly. Understanding CSS specificity is crucial for writing maintainable and predictable stylesheets.

## How to reproduce

1. Clone this repo
2. Create an HTML file like this:
```HTML
<div class="container">
  <p>This is some text.</p>
</div>
```
3. Link both `.css` files to your HTML file. Note the order may change the result.
4. Inspect the text's color. Note the unexpected red color.