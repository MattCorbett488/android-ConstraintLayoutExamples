
- MotionLayout can only provide capabilities for direct children (vs TransitionManager)

- Use MotionLayout when animating UI elements the user will interact with

- Has a property called progress - this is a float value (0 to 1) that defines what point the MotionScene is through the transition (0 to 100%)

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

Try and describe ConstraintSets in the MotionScene - noted for added functionality/future-proofing (future versions)

Each Constraint element will need all the constraints to apply to the widget (not a delta); if you only need to animate 1 widget out of a dozen, then only contain the constraint for that single widget