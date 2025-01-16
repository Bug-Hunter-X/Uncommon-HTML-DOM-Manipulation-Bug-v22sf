# Uncommon HTML DOM Manipulation Bug

This repository demonstrates an uncommon error in HTML where JavaScript code attempts to interact with the Document Object Model (DOM) before the page's DOM is fully loaded.  This can lead to unexpected errors and inconsistencies in the behavior of your web page.  The `bug.html` file shows the problematic code, and `bugSolution.html` provides the corrected version.

## Problem

In `bug.html`, the JavaScript attempts to hide the `div` element with id "myDiv" by setting its `display` style to "none". However, this happens before the browser has finished parsing and rendering the HTML, resulting in the JavaScript failing to find the element.  This leads to no changes in the webpage's visibility, even though the Javascript code executes without throwing any errors.