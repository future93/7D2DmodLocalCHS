# Bug Founded
## Bug 1
File **Localization.txt**:
Line **2-5**
### OriginalCode
`ocbBlockClaimAutoRepairDesc,UI,Menu,,,Automatically repairs blocks in its perimeter, within owner or allied claim, if the necessary materials are available in the container.`
### TroubleShoot
CSV files use commas to differentiate various values. Commas that are not used to separate values should be put in a pair of quotes. Also, tailing commas that have no values within shouldn't be removed.
### BugFix
`ocbBlockClaimAutoRepairDesc,UI,Menu,,,"Automatically repairs blocks in its perimeter, within owner or allied claim, if the necessary materials are available in the container.",,,,,,,,,,,,,,`

**This bug is already FIXED in the translated `Localization.txt` flie.**