### Transition tag

A tag that specifies the transition in a MotionScene

- Can be given an ID

- If changing an attribute via CustomAttribute tag, know that the attribute is not actually altered.  If you animate from 0 to 1 alpha, the widget animated will still have its original alpha - setting the alpha to 0 in the start Constraint and the alpha to 1 in the end Constraint will set the alpha to 1 after the animated transition.

Attributes:

- **constraintSetStart** used as start constraints (an ID) or layout file to get constraint from
- **constraintSetEnd** same as constraintSetStart but for end
- **interpolator** possible values: easeInOut, linear, anticipate, bounce, easeIn, easeOut
- **duration** length of time for the transition (in ms)
- **staggered** quick way to stagger the objects moving (float value)