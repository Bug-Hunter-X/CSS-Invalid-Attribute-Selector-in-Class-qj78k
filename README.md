# CSS Invalid Attribute Selector Bug

This repository demonstrates a common but easily overlooked error in CSS: using an attribute selector (like `[type="text"]`) on an element that doesn't possess such an attribute. This often leads to unexpected styling behavior.

## Problem
The `bug.css` file contains a CSS rule with the selector `.my-class[type="text"]`.  This is intended to style elements with the class `my-class` *and* a `type` attribute of "text", but this selector is invalid for elements that do not inherently possess `type` attributes, like `<div>` or `<span>`.

## Solution
The `bugSolution.css` file provides a corrected version where more appropriate selectors (e.g., class-based) are used to style the elements accurately. The solution depends on the intended HTML structure. This fix illustrates an alternative selection strategy for proper styling.