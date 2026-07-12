# ARCcalc HR1 v1.7

## Stability and history repairs

- Calculation History now stores and displays the full expression and calculated result separately.
- Negative weight values retain their sign while cycling units.
- Heat Input results are invalidated whenever any source parameter changes.
- Transferring a new IPM invalidates the previous Heat Input result.
- Switching from Stopwatch to Manual pauses the running timer.
- Clear removes saved Heat Input parameters from local storage.
- Reciprocal rejects dimensioned values until inverse-unit support exists.
- History and Settings dialogs now manage keyboard focus and Escape-to-close behavior.
- Removed the legacy iOS separator overlay and duplicate nested GCD declaration.
