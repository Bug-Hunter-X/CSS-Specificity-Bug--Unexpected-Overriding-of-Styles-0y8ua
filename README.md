# CSS Specificity Bug: Unexpected Overriding of Styles

This repository demonstrates an uncommon CSS bug related to specificity and the cascade.  The bug showcases a scenario where a more specific selector might not apply as expected due to the presence of other, even more specific selectors.

## Bug Description:

A seemingly straightforward CSS rule fails to apply as expected due to the unexpected behavior of CSS specificity and the cascade.  Higher specificity selectors override less specific selectors regardless of the order they are placed within the CSS file. In this example, a child selector may not function properly due to an outer selector applying to the same element with a higher level of specificity. 

## How to Reproduce:

1. Open `bug.css`.
2. Observe the unexpected behavior where the style application does not follow the expected cascade order. 

## Solution:

The solution involves carefully reviewing the CSS stylesheet to identify higher-specificity selectors that might be unintentionally overriding the expected styles.  Understanding CSS specificity and using developer tools to inspect the computed styles is crucial in debugging this type of issue. The `bugSolution.css` shows how to solve this problem by optimizing specificity.

## Technologies Used:

* CSS