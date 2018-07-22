
- Motionlayout can only provide capabilities for direct children (vs TransitionManager)

- Use MotionLayout when animating UI elements the user will interact with

MotionLayout automatically interpolates:

- Alpha
- Visibility
- Elevation
- Rotation, rotationX/Y
- translationX/Y/Z
- scaleX/Y

Possible attributes:
- **layoutDescription=“reference”** points to a MotionScene XML file e.x. app:layoutDescription=“@xml/scene_01”
- **applyMotionScene=“boolean”** is whether to apply the MotionScene (default: true)
- **showPaths=“boolean”** displays the motion path or not (default: false)
- **progress=“float”** specifies the transition progress (0 to 1)
- **currentState=“reference”** forces a specific ConstraintSet e.x. app:currentState=“@layout/constraint_set_layout_end”