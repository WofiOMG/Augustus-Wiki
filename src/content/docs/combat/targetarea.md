# TARGETAREA
Makes your character automatically strafe (circle-strafe) around the target during combat, improving movement and making it harder for enemies to hit you.

### X (Left ↔ Right):
Controls left and right movement.

Increasing X = move east/right.
Decreasing X = move west/left.

### Y (Up ↕ Down):
Controls vertical height.

Increasing Y = move up.
Decreasing Y = move down.

### Z (Forward ↔ Backward):
Controls forward and backward movement.

Increasing Z = move south/forward.
Decreasing Z = move north/backward.

**MinX:** 
Minimum distance left/right from the target's X position.
Negative values allow strafing far to the left.

**MaxX:**
Maximum distance right of the target's X position.
Allows strafing far to the right.

**MinY:**
Usually defines how far below the target you can be for strafing to activate.

**MaxY:** 
Maximum vertical height above the target where strafing is allowed.
255 = unrestricted (can strafe from below or above easily).

**MinZ:** 
Minimum forward/backward Z-range. This large value likely forces strafing to trigger only when very close.

**MaxZ:** 
Same as MinZ in this case — sets the valid range along the Z-axis (forward/backward) where TargetStrafe activates.

**Reverse:**
When true, inverts the defined area — strafing activates outside the given Min/Max bounds instead of inside.
Useful for enabling strafing only when far away, or to avoid being predictable.

