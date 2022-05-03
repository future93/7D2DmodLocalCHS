# Bug Founded
## Bug 1
File **Localization.txt**:
Line **10**
### OriginalCode
`modernCookingCharcoalGrillOpen,,blocks,Workstation,,,"Modern Charcoal Grill (Open)",,,,,,,,,,,,,,`
### TroubleShoot
`...GrillOpen,,blocks...` A surplus comma here. Should be 1 comma.
### BugFix
`modernCookingCharcoalGrillOpen,blocks,Workstation,,,"Modern Charcoal Grill (Open)",,,,,,,,,,,,,,`

**This bug is already FIXED in the translated `Localization.txt` flie.**
***
## Bug 2
File **Localization.txt**:
Line **12**
### OriginalCode
`modernCookingGasGrillOpen,blocks,Workstation,,,Modern "Modern Gas Grill (Open)",,,,,,,,,,,,,,`
### TroubleShoot
`...Workstation,,,Modern "Modern Gas...` A surplus "Modern" here.
### BugFix
`modernCookingGasGrillOpen,blocks,Workstation,,,Modern "Modern Gas Grill (Open)",,,,,,,,,,,,,,`

**This bug is already FIXED in the translated `Localization.txt` flie.**