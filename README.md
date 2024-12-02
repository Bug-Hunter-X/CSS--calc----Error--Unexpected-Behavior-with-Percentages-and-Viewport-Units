# CSS `calc()` Unexpected Behavior with Percentages and Viewport Units

This repository demonstrates an uncommon error that can occur when using the CSS `calc()` function with percentages and viewport units (vw) in a subtraction operation.  The issue lies in the potential for unexpected results or layout inconsistencies when combining these units within `calc()`, specifically in subtraction. 

## Bug Description
The provided CSS snippet aims to set an element's width to 50% of its parent's width minus 20% of the viewport width.  However, depending on the browser or context, the calculation within `calc()` may yield negative values or cause other layout problems.  This is likely due to inconsistencies in how different browsers interpret and handle these mixed units within `calc()`. 

## Solution
The most effective approach is to avoid combining percentage units and viewport units (or other relative units) within subtraction operations in `calc()`. Instead, a more reliable method involves using a different approach to achieve the desired layout.