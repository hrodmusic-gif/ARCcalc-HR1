# ARCcalc HR1 v1.6

## Stability repairs

- Preserves sufficient decimal precision for valid very-low travel-speed results instead of rounding them to zero.
- Transfers the same nonzero precision into Heat Input.
- Clears and disables an old IPM result whenever a new stopwatch timing run begins or the stopwatch is reset.
- Keeps IPM calculations inside the Travel Speed result panel so they no longer replace the Heat Input Result screen.

## Settings and accessibility

- Calculator Guide is collapsed by default and opens only when requested.
- Increased the calculation-history and bottom-tab touch targets to at least 44 CSS pixels on phones.

## Package cleanup

- Removed four unused source/overlay images from the production PWA package.
- Existing calculator, stair, weight, shape, history, unit-conversion, heat-input, and IPM formulas remain unchanged except for IPM display/transfer precision.
