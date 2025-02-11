# CSS Specificity and !important Conflict

This repository demonstrates a subtle and uncommon bug related to CSS specificity and the `!important` declaration.  The issue arises when a selector with `!important` overrides a more specific selector.

## Bug Description

The `!important` flag in CSS allows overriding almost any specificity rule, even if a selector is more specific. This can cause unexpected behavior and make debugging difficult.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` and observe the CSS selectors.
3. Inspect the HTML element (using browser developer tools) to see the unexpected outcome.

## Solution

The solution involves avoiding the unnecessary use of the `!important` flag wherever possible.  Use more specific selectors to achieve the desired styling instead of relying on `!important`.

See `bugSolution.css` for a corrected example.