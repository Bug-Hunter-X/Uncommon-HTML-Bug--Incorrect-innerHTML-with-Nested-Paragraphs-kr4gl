# Uncommon HTML Bug: Incorrect innerHTML with Nested Paragraphs

This repository demonstrates an uncommon bug related to setting the `innerHTML` property in HTML.  The issue arises when attempting to inject HTML containing nested paragraph tags (`<p>`) directly into an element's `innerHTML`.  Browsers might handle this incorrectly, leading to unexpected rendering issues.

The `bug.html` file showcases the problem, while `bugSolution.html` presents the corrected approach, illustrating how to handle nested elements safely using DOM manipulation techniques.

## Bug Description

The main issue lies in directly assigning nested HTML elements using `innerHTML`. The browser might not properly parse or render the nested structure, causing the visual output to differ from the intended result.  Improper nesting often leads to unexpected results.  This can be particularly confusing for developers unfamiliar with this subtle HTML parsing behavior.

## Solution

The solution involves using DOM manipulation to construct the HTML elements programmatically instead of relying solely on `innerHTML`. This provides better control and avoids potential rendering issues arising from parsing nested structures directly into `innerHTML`.