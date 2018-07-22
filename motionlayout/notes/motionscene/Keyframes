### Keyframes

Keyframes allow us to manipulate the path of one or more objects during animation.  While we specify the start constraints and the end constraints, Keyframes let us manipulate the layout between the start and end

3 primary tags:
- KeyPosition: lets you change the shape of the path
- KeyAttribute: used with standard view attributes or custom attributes, lets you manipulate attributes along the path
- KeyCycle: controls oscillations (frequency and type) during animation

To specify multiple Keyframes, put them in a <KeyFrameSet\> tag

#### KeyPosition

Example:
```markdown
<KeyPosition
    motion:type="pathRelative"
    motion:percentY="-0.25"
    motion:framePosition="50"
    motion:target="@id/button"/>
```

This example will cause the `button` widget (the `target` of this KeyPosition tag), to move up the Y axis 25% (by specifying the `percentY`) and this occurs at the halfway point (`framePosition` is the percent [0-100] where the KeyPosition occurs)

The `type` attribute can be either `deltaRelative` (relative to the Y axis in this case) or `pathRelative`


#### KeyAttribute

Used to manipulate attributes at certain points along the path.

Example:
```markdown
<KeyAttribute
    android:scaleX="2"
    android:scaleY="2"
    android:rotation="-45"
    motion:framePosition="50"
    motion:target="@id/button" />
```

This example will scale both the X and Y of the button to 200% while also rotating it by -45 degrees. We can use normal view attributes here, or we could also nest a <CustomAttribute\> tag

### KeyCycle

If we want any custom oscillations along our path, the KeyCycle tag has multiple pre-defined oscillations

Example:
```markdown
<KeyCycle
    android:translationY="50dp"
    motion:framePosition="50"
    motion:target="@id/button"
    motion:waveOffset="0"
    motion:wavePeriod="1"
    motion:waveShape="sin" />
```

The main 3 attributes here are the `waveOffset`, the `wavePeriod` for the number of cycles to loop in the region, and the `waveShape` for what the wave should look like.

This example produces a sin wave with a period of 1 at the halfway point in the path

Possible `waveShape` values:
- sin
- square
- triangle
- sawtooth
- reverseSawtooth
- cos
- bounce

We can also include <CustomAttribute\> tags here if we want