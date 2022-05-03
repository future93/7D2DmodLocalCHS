# Bug Founded
## Bug 1
File **Localization.txt**:
Line **9**
### OriginalCode
`rollingGarageDoorBrownDesc,blocks,Block,,,,A rolling overhead Garage Door that can be locked.\nUsing the default placement you are standing on the outside and it will open by rolling up and away from you.\nRepair with Forged Iron.,,,,,,,,,,,`
### TroubleShoot
`...Desc,blocks,Block,,,,A rolling...` A surplus comma here. Should be 3 commas.
### BugFix
`rollingGarageDoorBrownDesc,blocks,Block,,,A rolling overhead Garage Door that can be locked.\nUsing the default placement you are standing on the outside and it will open by rolling up and away from you.\nRepair with Forged Iron.,,,,,,,,,,,`

**This bug is already FIXED in the translated `Localization.txt` flie.**