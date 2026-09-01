# GroundObject - Unity editor utility
## How it works
Download __GroundObject.unitypackage__.
This package contains three C# scripts: GroundObject, GroundObjectHandler and GroundObjectEditor.

In your HDRP, BIRP or URP project import downloaded file thru Assets/Import Package.

Add Component __Ground Object__ to your scene object. Adjust __xSize__, __ySize__ and turn on or off cells appeared beneath your object. 
The cells are turned on by default. When you turn them off they became more transparent. Dragging works for mass painting.
This way your can visually set bounds for your object and transfer that information to your game engine thru field __occupiedArray__.
This would be useful when you generate level and randomly add different ground objects to your scene so that they are not touching each other.

When you add __Ground Object__ to your scene object, helper object named __Ground object editor handler__ is added to scene. Two helper materials named __NormalGroundMat__ and __FadedGroundMat__ added to __Assets/Resources/Materials__. 
When you have no objects in your scene with component __Ground Object__, you can delete those helper objects.
